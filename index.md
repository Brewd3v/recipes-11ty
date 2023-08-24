---
layout: "layouts/base.njk"
title: Recipe Book
eleventyExcludeFromCollections: true
eleventyImport:
  collections: ["recipe"]
---

# Recipe Book 11

<ul>
{%- for recipe in collections.all -%}
  <li><a href="{{ recipe.url }}">{{ recipe.data.title }}</a></li>
{%- endfor -%}
</ul>