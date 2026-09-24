# Modelos de Prática Profissional — IFRN Campus Ceará-Mirim

Site estático (GitHub Pages) com o guia e os modelos de artigo/relatório da
Prática Profissional do Técnico Integrado em Informática (PPC 2012), para os
alunos baixarem diretamente — sem depender de link do Drive.

**Site:** https://jp-guimaraes.github.io/modelos-rpp-ifrn-cm/ (depois de
habilitar o GitHub Pages em Settings → Pages → Branch: `main` / `/ (root)`)

## Estrutura

- `index.html`, `modelos.html`, `mostra-2026.html`, `overleaf.html`, `faq.html` — páginas do site (HTML puro, sem build).
- `assets/css/style.css` — estilo único, compartilhado por todas as páginas.
- `assets/img/` — logo do IFRN usado no cabeçalho.
- `files/<modalidade>/` — os arquivos para download (`.docx`, `.pdf`, `.tex`), um subdiretório por modalidade (`pesquisa/`, `estagio/`, `extensao/`, `mostra-2026/`). `pesquisa/` e `mostra-2026/` também têm uma cópia de `ifrn-logo.png`, exigida pelos `.tex` que usam o símbolo no cabeçalho/capa (ver `overleaf.html`).

## Como atualizar

Os modelos-fonte vivem em `Coordenação INFO/08-Pratica-Profissional/` (fora
deste repositório). Para atualizar um arquivo aqui:

1. Edite o modelo na origem (`Coordenação INFO/08-Pratica-Profissional/<modalidade>/modelos/`).
2. Copie o arquivo atualizado para `files/<modalidade>/` neste repositório.
3. Se a estrutura/metadado mudou, atualize também o texto correspondente em `modelos.html` (ou `mostra-2026.html`).
4. Commit e push.

Não há build step — é só HTML/CSS estático, o GitHub Pages serve direto.
