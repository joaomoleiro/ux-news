# UX News

Site Jekyll de exemplo com listagem de posts e página de detalhe.

## Correr localmente

```bash
bundle install
bundle exec jekyll serve
```

Abre `http://localhost:4000`.

## Estrutura

```
_config.yml       Configuração do site
_layouts/         Templates (default.html, post.html)
_posts/           Artigos em Markdown (YYYY-MM-DD-titulo.md)
assets/style.css  Estilos
index.html        Página de listagem
```

## Adicionar um post

Cria um ficheiro em `_posts/` com o nome `AAAA-MM-DD-titulo.md` e o front matter:

```yaml
---
layout: post
title: "O título"
date: 2026-06-29
author: João Moleiro
categoria: "irAuthor web"   # opcional
---

Conteúdo em Markdown.
```

## Publicar no GitHub Pages

1. Faz push deste repositório para o GitHub.
2. Em **Settings → Pages**, escolhe o branch (ex.: `main`) e a pasta `/ (root)`.
3. O GitHub faz o build automaticamente com a gem `github-pages`.

Se o site for servido a partir de `utilizador.github.io/uxnews`, define no `_config.yml`:

```yaml
baseurl: "/uxnews"
```
