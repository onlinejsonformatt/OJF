# Parquet Viewer Online — View Apache Parquet Files in Your Browser

**Live tool:** [https://www.onlinejsonformatt.org/en/parquet-viewer-online](https://www.onlinejsonformatt.org/en/parquet-viewer-online)

Open and inspect Apache Parquet files directly in the browser — no Python, no Spark, no installation required.

---

## Why This Exists

Apache Parquet is the dominant columnar format for big data, but viewing a `.parquet` file typically requires:
- Installing Python + pandas/pyarrow
- Setting up a Jupyter notebook
- Or using DuckDB/Spark CLI

This tool eliminates all of that. **Drag, drop, view** — in seconds, in your browser.

---

## What Makes This Different

| Feature | OJF Parquet Viewer | Alternatives |
|---------|:---:|:---:|
| No installation (runs in browser) | Yes | Requires Python/CLI |
| 100% client-side (file never uploaded) | Yes | Some upload to servers |
| Column inspection (names, types, nulls) | Yes | Varies |
| Row preview with pagination | Yes | Usually requires code |
| Works on mobile/tablet | Yes | Desktop-only tools |
| Free, no signup | Yes | Varies |

---

## Supported Parquet Features

| Feature | Support |
|---------|---------|
| Snappy compression | Yes |
| Gzip compression | Yes |
| Uncompressed | Yes |
| Nested schemas (struct/list/map) | Yes |
| Multiple row groups | Yes |
| Null handling | Yes |
| Date/time types | Yes |
| Decimal types | Yes |

---

## How It Works

```
┌──────────────────────────────────────────────┐
│  1. Drag & drop .parquet file                │
│         │                                     │
│         ▼                                     │
│  2. Client-side Parquet parser (WebAssembly)  │
│         │                                     │
│         ▼                                     │
│  3. Schema extraction                         │
│     • Column names and data types             │
│     • Row group metadata                      │
│     • Compression info                        │
│         │                                     │
│         ▼                                     │
│  4. Tabular display with pagination           │
│     • Sort, scroll, inspect values            │
│     • No limit on columns                     │
└──────────────────────────────────────────────┘
```

All parsing happens in your browser using WebAssembly — the file is never uploaded anywhere.

---

## Common Use Cases

- **Data engineering** — Quick-check Parquet exports without spinning up a notebook
- **ETL debugging** — Verify pipeline output schema and row counts before loading to warehouse
- **Data science** — Preview datasets before committing to a full pandas/Spark workflow
- **QA validation** — Confirm data types, null patterns, and column structure in CI artifacts
- **Teaching** — Demonstrate columnar storage concepts without requiring students to install tools
- **Ad-hoc exploration** — "What's in this Parquet file?" answered in 3 seconds

---

## Privacy & Security

Your Parquet file never leaves your machine. The viewer parses the file entirely in-browser using WebAssembly. No server receives your data — safe for proprietary datasets, PII-containing files, and internal analytics exports.

---

## Try It

1. Open [Parquet Viewer](https://www.onlinejsonformatt.org/en/parquet-viewer-online)
2. Drag-and-drop a `.parquet` file (or click to browse)
3. View schema, column types, and row data instantly
4. Navigate pages for large datasets

No Python. No Spark. No signup. No data upload.

---

## Related Tools

- [JSON Formatter](../json-formatter-online/README.md) — Format JSON output from data pipelines
- [JSON to CSV](../json-to-csv/README.md) — Convert JSON to spreadsheet format
- [Blog](../blogs/README.md) — Guides on Parquet, data formats, and tooling
- [Back to all tools](../README.md)
