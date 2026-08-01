# JSON Tree View — Visual Hierarchy Explorer

**Live tool:** [https://www.onlinejsonformatt.org/en/tree-view](https://www.onlinejsonformatt.org/en/tree-view)

Visualize JSON as an interactive, collapsible tree — navigate deeply nested structures without reading raw text.

---

## What Makes This Different

| Feature | OJF Tree View | Text-based formatters |
|---------|:---:|:---:|
| Interactive expand/collapse nodes | Yes | Static indentation |
| Search within tree | Yes | Find in text only |
| Type indicators (string, number, bool, null) | Yes | Color-only |
| Array length & object key count at a glance | Yes | Must count manually |
| Path copy (click node → copy JSON path) | Yes | No |
| 100% client-side (no data upload) | Yes | Varies |

---

## Key Features

### Visual Navigation
- **Expand/collapse** — Click any object or array to expand or fold its children
- **Type badges** — Instantly see whether a value is a string, number, boolean, null, object, or array
- **Size indicators** — Objects show key count, arrays show element count without expanding
- **Depth highlighting** — Visual nesting levels help orient you in deeply nested documents

### Search & Discovery
- **Tree search** — Find keys or values anywhere in the structure
- **Path display** — See the full JSON path (e.g., `data.users[0].name`) for any selected node
- **Path copy** — One-click copy of the path for use in code, JMESPath, or jq filters

### Developer Workflow
- **Paste or drag-drop** — Load JSON instantly
- **Large document support** — Handles thousands of nodes with virtualized rendering
- **Keyboard navigation** — Arrow keys to traverse, Enter to expand/collapse
- **Works alongside formatter** — Switch between tree and text views of the same data

---

## How It Works

```
Input JSON:
{
  "users": [
    {"name": "Alice", "role": "admin"},
    {"name": "Bob", "role": "dev"}
  ],
  "meta": {"count": 2}
}

Tree View:
▼ root {3 keys}
  ▼ users [2 items]
    ▼ [0] {2 keys}
        name: "Alice"    (string)
        role: "admin"    (string)
    ▶ [1] {2 keys}
  ▼ meta {1 key}
      count: 2           (number)
```

---

## Common Use Cases

- **API response exploration** — Understand complex nested payloads from REST/GraphQL endpoints
- **Schema discovery** — See the shape of unfamiliar JSON without reading documentation
- **Debugging** — Locate a specific nested value by expanding the tree instead of scrolling text
- **Documentation** — Screenshot the tree view to illustrate data structures in docs/wikis
- **Teaching** — Show students how JSON nesting works visually
- **Config inspection** — Navigate large config files (webpack, tsconfig, package.json) by section

---

## Privacy & Security

All tree rendering happens in your browser. Your JSON is parsed and displayed client-side — no server ever receives your data. Safe for sensitive payloads, API keys, and internal data structures.

---

## Try It

1. Open [Tree View](https://www.onlinejsonformatt.org/en/tree-view)
2. Paste JSON or drag-drop a `.json` file
3. Click nodes to expand/collapse
4. Use search to find specific keys or values
5. Click any node to copy its JSON path

No signup. No limits. No data leaves your browser.

---

## Related Tools

- [JSON Formatter](../json-formatter-online/README.md) — Text-based pretty-print view
- [Editor](../editor/README.md) — Edit JSON with IDE features
- [Compare](../compare/README.md) — Diff two JSON structures
- [Fix JSON](../fix-json/README.md) — Repair broken JSON before viewing
- [Back to all tools](../README.md)
