---
tags:
  - indexNoteType
aliases: []
date: "{{date}} {{time}}"
image: ""
---
>[!info] How To Use
>**Quick Guide**
>1. name me like this: `$(name of the index) Index (emoji)` 
>2. write a quote or description in the quote callout (change it's type if needed)
>3. edit the yaml properties as you wish, just leave `date` and `indexNoteType` tag as is
>4. link a note to this index, it will show up in the [[#Inbox]] base, when shown, link it again in the [[#Index Items]] links, you can also search index notes by first writing a dollar sign $
>5.  remove me (this callout block) when done
>
>**What is it**
>an index note type (aka MoC note) is meant to be an index or a collection of notes, think of it like a folder or phone book, it is used to keep track of and organize all types of notes in your PKM system or zettle kasten.
>
>you can make index notes about anything, maybe you want to organize notes taken about your development project or any project, you can make an index for it, or index for notes about ideas, or index for book summaries, etc, you can make an index for any
# {{title}}
---
- ***Index links:*** [[]], [[]]

> [!quote] Quote
> write a Quote or a sentence...
> - by you
## Inbox
```base
filters:
  and:
    - file.hasLink(this.file)
    - not:
        - this.file.links.contains(file.asLink())
views:
  - type: list
    name: index links
    order:
      - file.name
      - file.tags

```
## Index Items
- links
  - [[]]
