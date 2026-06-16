# Revista Tempovani

Site da Revista Tempovani — um espaço para publicar artigos, inspirado no estilo da revista piauí.

## Como publicar

### 1. Criar um artigo novo

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
categories: [categoria]
---

Texto do artigo em Markdown...
```

### 2. Estrutura de categorias (opcional)

Você pode usar categorias como: `editorial`, `crônica`, `política`, `cultura`, `ciência`, `literatura`, `reportagem`, etc.

## Deploy no GitHub Pages

Crie um repositório **novo e separado** chamado `revista-tempovani`:

```bash
git init
git add .
git commit -m "Revista Tempovani"
git remote add origin https://github.com/tempxrin/revista-tempovani.git
git push -u origin main
```

No GitHub, vá em **Settings > Pages** e selecione a branch `main`.

O site estará em: **`https://tempxrin.github.io/revista-tempovani`**

> O `baseurl` já está configurado como `/revista-tempovani`.

## Domínio personalizado

Para usar um domínio bonito (ex: `revista.tempovani.com.br`):

1. Compre o domínio em qualquer registradora
2. No seu repositório, vá em Settings > Pages > Custom domain
3. Adicione seu domínio e salve
4. Na sua registradora, crie os registros DNS:
   - **A** apontando para `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Ou **CNAME** apontando para `tempxrin.github.io`

> OBS: Domínios `.com.br` custam ~R$ 40/ano em registradoras como registro.br, HostGator, etc.

## Desenvolvimento local

```bash
# Instalar Jekyll e Bundler
gem install jekyll bundler

# Instalar dependências
bundle install

# Rodar servidor local
bundle exec jekyll serve
```

Acesse `http://localhost:4000`

## Estilo

Layout inspirado na [revista piauí](https://piaui.uol.com.br/), com:

- **Playfair Display** para o logo
- **Merriweather** para títulos e texto corrido
- **Inter** para elementos de navegação
- Paleta: fundo quente (#f9f6f2), texto sóbrio (#1a1a1a), acento terracota (#d4785c)
