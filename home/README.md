# Online JSON Formatt - The Privacy-First Developer Toolkit

**Live site:** [https://www.onlinejsonformatt.org](https://www.onlinejsonformatt.org)

A free, browser-based suite of 17+ JSON, XML, and data tools - powered by AI, built on privacy, available in 6 languages.

---

## What Is Online JSON Formatt?

Online JSON Formatt (OJF) is a developer-focused platform that provides formatting, validation, repair, comparison, conversion, and visualization tools for structured data - all running 100% in your browser.

Unlike traditional online tools that send your data to a server for processing, OJF processes everything client-side. Your JSON, XML, and Parquet files never leave your machine.

---

## The Complete Tool Suite

### JSON Tools (7 tools)

| Tool | Purpose | Unique Angle |
|------|---------|--------------|
| [Formatter](../json-formatter-online/README.md) | Pretty-print and beautify JSON | Monaco Editor, 10MB+ support |
| [Editor](../editor/README.md) | Full IDE for JSON editing | VS Code engine, JMESPath filtering |
| [Tree View](../tree-view/README.md) | Visual hierarchy explorer | Expand/collapse, search within tree |
| [Compare](../compare/README.md) | Structural diff for JSON | JSON-aware (not line-based) |
| [Fix JSON](../fix-json/README.md) | AI-powered repair | 7-layer engine, fixes multiple errors |
| [Escape](https://www.onlinejsonformatt.org/en/json-escape-online) | Escape/unescape strings | Handles all escape sequences |
| [Minify](../minify/README.md) | Compress for production | Whitespace removal, size reporting |

### Converters (6 tools)

| Tool | Direction | Output |
|------|-----------|--------|
| [JSON → XML](../json-to-xml/README.md) | JSON to XML | Well-formed XML with declaration |
| [XML → JSON](../xml-to-json/README.md) | XML to JSON | Clean JSON from any XML |
| [JSON → CSV](../json-to-csv/README.md) | JSON to CSV | Flattened tabular data |
| JSON → YAML | JSON to YAML | Human-readable config format |
| JSON → POJO | JSON to Java classes | Type-safe model generation |
| JSON → Dart | JSON to Dart classes | Flutter model generation |

### XML Tools (4 tools)

| Tool | Purpose |
|------|---------|
| XML Formatter | Pretty-print XML with indentation |
| [XML Compare](https://www.onlinejsonformatt.org/en/xml-compare) | Structural diff for XML documents |
| XML → CSV | Flatten XML into spreadsheet format |
| [XML → JSON](../xml-to-json/README.md) | Convert XML to JSON structure |

### Data Tools

| Tool | Purpose | Unique Angle |
|------|---------|--------------|
| [Parquet Viewer](../parquet-viewer-online/README.md) | View Apache Parquet in browser | No Python/Spark required |

---

## Why Developers Choose OJF

### 1. Privacy by Design
Every tool runs **100% in your browser**. No data upload, no server processing, no telemetry on your input. Safe for API keys, tokens, PII, and proprietary data.

### 2. AI-Powered Repair
The Fix JSON tool uses a **7-layer repair engine** that automatically fixes broken JSON - trailing commas, unquoted keys, single quotes, unclosed brackets, and more. No other free tool offers this depth of automated repair.

### 3. Professional Editor
Built on **Monaco Editor** (the same engine as VS Code) - code folding, multi-cursor, regex find/replace, inline error highlighting, and syntax awareness that textarea-based tools can't match.

### 4. Multilingual
Full interface in **6 languages**: English, French, Spanish, German, Russian, and Dutch. Not just translated buttons - full SEO content, FAQs, and documentation in each language.

### 5. Comprehensive Suite
17+ tools in one place. Format, validate, repair, compare, convert, visualize - without juggling between different sites for each operation.

### 6. No Friction
No signup, no account, no API key, no rate limits. Open a tool and use it. Free forever.

---

## Technical Architecture

| Layer | Technology |
|-------|-----------|
| Framework | Next.js 14+ (App Router, Server Components) |
| Editor | Monaco Editor (VS Code engine) |
| Rendering | Server-side rendering for SEO + client-side for interactivity |
| AI Repair | Custom 7-layer heuristic pipeline (client-side) |
| Parquet | WebAssembly-based parser (no server) |
| Structured Data | JSON-LD (Organization, WebApplication, FAQ, HowTo, BreadcrumbList) |
| i18n | 6 locales with full hreflang implementation |
| Performance | Code splitting, lazy loading, optimized Core Web Vitals |

---

## Who Uses This

- **Backend developers** - API debugging, payload validation, JSON repair from flaky endpoints
- **Frontend developers** - Formatting API responses, filtering nested data, config editing
- **Data engineers** - Parquet viewing, format conversion (JSON ↔ CSV ↔ XML), pipeline debugging
- **DevOps engineers** - Config comparison, minification for deployments, schema validation
- **QA engineers** - Test data comparison, expected-vs-actual JSON diffing
- **Students** - Learning JSON structure, data format exploration, coursework tools

---

## Content & Resources

The [blog](../blogs/README.md) publishes tutorials and guides including:
- Format Large JSON Files Without Crashing
- Getting Reliable JSON Output from LLMs
- JSON Validation Best Practices
- JSON to CSV Conversion Guide
- Everything You Need to Know About JSON

---

## Getting Started

1. Visit [onlinejsonformatt.org](https://www.onlinejsonformatt.org)
2. Pick a tool from the homepage grid
3. Paste or drag-drop your data
4. Get instant results - no signup required

---

## Links

- **Website:** [onlinejsonformatt.org](https://www.onlinejsonformatt.org)
- **GitHub:** [github.com/onlinejsonformatt](https://github.com/onlinejsonformatt)
- **Blog:** [onlinejsonformatt.org/en/blogs](https://www.onlinejsonformatt.org/en/blogs)
- **About:** [onlinejsonformatt.org/en/about](https://www.onlinejsonformatt.org/en/about)
- **Contact:** [onlinejsonformatt.org/en/contact](https://www.onlinejsonformatt.org/en/contact)

---

## Related Pages

- [All tools (hub)](../README.md)
- [About the project](../about/README.md)
- [Blog index](../blogs/README.md)
- [Contact](../contact/README.md)
