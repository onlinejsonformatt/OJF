# JSON Compare — Side-by-Side Diff for JSON Payloads

**Live tool:** [https://www.onlinejsonformatt.org/en/compare](https://www.onlinejsonformatt.org/en/compare)

Compare two JSON documents visually — see additions, deletions, and modifications highlighted in a side-by-side or inline diff view.

---

## What Makes This Different

| Feature | OJF Compare | Text-based diff tools |
|---------|:---:|:---:|
| JSON-aware structural diff | Yes | Line-by-line only |
| Handles key reordering gracefully | Yes | Shows false positives |
| Nested object/array comparison | Yes | Flattened view |
| Side-by-side + inline views | Yes | Usually one mode |
| 100% client-side (no data upload) | Yes | Many use servers |
| Syntax highlighting in diff | Yes | Plain text |
| Free, no signup | Yes | Freemium |

Standard text diff tools (like Unix `diff`) compare line-by-line — so reordering JSON keys shows everything as "changed" even when semantically nothing is different. This tool understands JSON structure and diffs at the **value level**, not the text level.

---

## Diff Output Explained

```
Left (Original)              Right (Modified)
─────────────────            ─────────────────
{                            {
  "name": "Alice",     ≠       "name": "Bob",          ← Modified
  "age": 30,           =       "age": 30,              ← Unchanged
  "role": "dev"        -                                ← Deleted
                        +       "team": "platform"      ← Added
}                            }
```

The tool highlights:
- **Green** — Added keys/values (exist in right, not in left)
- **Red** — Removed keys/values (exist in left, not in right)
- **Yellow/Orange** — Modified values (same key, different value)
- **Unchanged** — Identical content shown for context

---

## Key Features

### Structural Awareness
- Compares objects by **key**, not by line position
- Arrays compared element-by-element with smart alignment
- Nested diffs — changes 5 levels deep are highlighted correctly

### Comparison Modes
- **Side-by-side** — Both documents visible simultaneously
- **Inline** — Unified diff with additions/deletions interleaved
- **Summary** — Quick count of additions, deletions, modifications

### Developer Workflow
- Paste two JSON payloads (left = original, right = modified)
- Drag-and-drop two `.json` files
- Swap sides with one click
- Format both sides before comparing

---

## Common Use Cases

- **API versioning** — Compare responses between API v1 and v2
- **Config changes** — Review what changed in deployment configs before merging
- **Database snapshots** — Diff JSON exports from different time periods
- **Test assertions** — Compare expected vs. actual JSON output from tests
- **Code review support** — Visualize JSON schema changes in PRs
- **Debugging** — Find the one field that changed between "working" and "broken" states

---

## Privacy & Security

Both JSON documents stay in your browser. No data is sent to any server — safe for comparing sensitive configs, API keys, internal payloads, and production data.

---

## Try It

1. Open [JSON Compare](https://www.onlinejsonformatt.org/en/compare)
2. Paste or drop JSON into the left (original) and right (modified) panels
3. View the structural diff with color-coded highlights
4. Toggle between side-by-side and inline views

No signup. No limits. No data leaves your machine.

---

## Related Tools

- [JSON Formatter](../json-formatter-online/README.md) — Format JSON before comparing
- [Fix JSON](../fix-json/README.md) — Repair broken JSON so it can be compared
- [Tree View](../tree-view/README.md) — Explore structure visually
- [Editor](../editor/README.md) — Edit JSON with IDE features
- [Back to all tools](../README.md)
