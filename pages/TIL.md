---
content-type: note
notetype : unfeed
permalink: /til
date: 2022-02-15 22:02:00
title: The things I learnt while setting up Metathinkr Garden
---
# The things I learnt while setting up Metathinkr Garden
## things that obstruct build:
1. The `yaml` thing can be obstrutive for build. Be careful when using `keys`. For example: `date` key has one and only one way to write. Also Never leave the value of date key empty
2. The traditional `<!--comment-->` won't work. Instead use `{%- comment -%}` `{%- endcomment -%}`. Jekyll will use `{{`include xyz.html`}}` anyway in traditional comments.
## things specific to Obsidian
1. The linter plugin by @platers has an auto yaml intserter. Be careful to not leave a space between `key` and `:`. eg
```yaml
notetype : #eg unfeed or feed
```
will create (upto two) duplicates at every save, hence wrong result. Notice the space before colon.
```yaml
notetype: #eg unfeed or feed
```
will work right.
