
---
notetype : #eg unfeed or feed
permalink: /til
date: 2022-02-15 22:02:00
title: The things I learnt while setting up Metathinkr Garden
---
# The things I learnt while setting up Metathinkr Garden
## things that obstruct build:
1. The `yaml` thing can be obstrutive for build
2. The 
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
