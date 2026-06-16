# revista sinedoque

Site da revista sinedoque.

## Como publicar

Crie um arquivo `.md` na pasta `_posts/` seguindo o formato:

```
_posts/AAAA-MM-DD-titulo-do-artigo.md
```

Exemplo:
```markdown
---
title: "Título do Artigo"
author: "Seu Nome"
date: 2026-06-20
categories: [cultura]
---

Texto do artigo em Markdown...
```

### Categorias disponíveis

- `politica`
- `economia`
- `cultura`

## Deploy

O deploy é automático via Cloudflare Pages — a cada push na branch `main`.

## Desenvolvimento local

```bash
bundle install
bundle exec jekyll serve
```

Acesse `http://localhost:4000`
