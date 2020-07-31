---
title: "A periodic table of elements in multiple languages"
slug: multilingual-periodic-table
description: A pretty and printable periodic table in Tex/LaTex in various languages
date: 2020-07-31T11:29:25+02:00
type: posts
draft: false
categories:
- sciences
languages:
- RU/FR
- RU/EN
- FR/EN
---

Salut

<ul>
  {{ $dataJ := getJSON "https://api.github.com/repos/StorkST/multilingual-periodic-table/releases/tags/1.0.1" }}
    {{ $assets := .assets }}
      {{ range first 2 $assets }}
        <li>{{ .label }}</li>
      {{ end }}
</ul>
