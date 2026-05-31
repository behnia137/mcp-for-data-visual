# 🤝 Contributing to MCP for Data Professionals — Visual Edition

First off: **thank you!** This project gets better every time someone adds a clearer analogy or a missing concept. You don't need to be an MCP expert — if you can explain something simply, you can contribute.

---

## 🌟 Ways to contribute

- **Add a new concept** (the most valuable!)
- **Improve an existing analogy** — make it clearer or more memorable
- **Fix or upgrade a diagram**
- **Fix typos / grammar / broken links**
- **Translate** a concept into another language

---

## ✍️ Adding a new concept

Each concept is **one markdown file** in the [`/data`](data) folder. Keep filenames lowercase with hyphens, e.g. `mcp-databricks.md`.

### Copy this template

```markdown
# {EMOJI} {Title}

> **🧒 Explain Like I'm 5:** {One friendly sentence.}

## 🖼️ The Picture

```mermaid
flowchart LR
    A["Node A"] --> B["Node B"]
    style A fill:#fef3c7,stroke:#f59e0b,color:#1f2937
    style B fill:#dcfce7,stroke:#22c55e,color:#1f2937
```

{One sentence caption.}

## 🔧 How it actually works

{2-3 short paragraphs, plain language}

## 🌍 Real-world example

{One concrete paragraph — data context}

## 🔗 Related

- [Concept](filename.md)
```

### Then

1. Add your file to `/concepts`.
2. Add a row to the README table with the emoji, link, and one-liner.
3. Open a Pull Request.

---

## ✅ Style guide

- **Analogy first** — the ELI5 line should be the first thing a reader sees
- **Diagram required** — every concept needs a Mermaid flowchart
- **Short paragraphs** — aim for 3-5 sentences max per paragraph
- **Beginner-readable** — avoid jargon without explanation; if you must use a term, define it in one sentence
- **Data context** — real-world examples should be grounded in Power BI, Fabric, SQL, Excel, or Python data work
- **Consistent Mermaid colors** — use only the palette below

### Mermaid color palette

| Color | Use for | Values |
|-------|---------|--------|
| 🟡 Yellow | Key / central nodes | `fill:#fef3c7,stroke:#f59e0b,color:#1f2937` |
| 🔵 Blue | Input / neutral nodes | `fill:#dbeafe,stroke:#3b82f6,color:#1f2937` |
| 🟢 Green | Output / positive result | `fill:#dcfce7,stroke:#22c55e,color:#1f2937` |
| 🔴 Red | Error / warning | `fill:#fee2e2,stroke:#ef4444,color:#7f1d1d` |

Do not use other colors. Consistent styling makes the whole repo feel like one coherent resource.

---

## 🔁 Pull Request checklist

Before opening a PR, confirm:

- [ ] File is in `/concepts` with a lowercase hyphenated filename
- [ ] File follows the 5-section template (ELI5, Picture, How it works, Real-world, Related)
- [ ] Mermaid diagram uses only the approved color palette
- [ ] README table row added with correct emoji, link, and one-liner
- [ ] No broken links
- [ ] Paragraphs are short and beginner-readable
- [ ] Real-world example is grounded in a data professional context

---

## 💬 Not sure where to start?

Good first additions: MCP + Databricks, MCP + Snowflake, MCP + dbt, MCP + Azure Data Factory, MCP transport types (stdio vs SSE), MCP logging and observability.

Open an issue if you want to claim a concept before writing it — that way two people don't work on the same thing at the same time.

Thanks for helping data professionals connect AI to their stack. 🔌💛
