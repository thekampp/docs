> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

- **Atleta** (pt-BR) / **athlete** (en) — nunca "aluno", "cliente" ou "client".
- **Anamnese** (pt-BR) / **intake form** (en) — o questionário configurável do coach.
- **Avaliação física** (pt-BR) / **assessment** (en) — medidas, dobras e fotos. É outra coisa.
- **Treino** = a sessão; **pasta** = o que se entrega. Entrega é sempre por pasta.
- **Coach** (os dois idiomas) — não "treinador" nos títulos de menu.

## Style preferences

{/* Add any project-specific style rules below */}

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Documente só o que o coach vê no painel (`kampp-coach`) e o que o atleta vê no app.
- Não documente o backoffice interno (`kampp-admin`) nem detalhes de API/infra.
- Toda página existe nos **dois idiomas** (`pt-BR/` e `en/`) e nos dois grupos do `docs.json`.
- Ao renomear um arquivo, adicione o `redirect` correspondente no `docs.json`.
