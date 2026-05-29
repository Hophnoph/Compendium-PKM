>[!quote] Quote
>“He who has a why to live can bear almost any how.”
— Friedrich Nietzsche

---
# ⚡️ Activity Feed ⚡️
```base
filters:
  and:
    - file.ext == "md"
formulas:
  last_edited: file.mtime.relative()
properties:
  file.name:
    displayName: Note
  formula.last_edited:
    displayName: Last edited
views:
  - type: table
    name: Recently edited notes
    order:
      - file.name
      - formula.last_edited
    sort:
      - property: file.mtime
        direction: DESC
    limit: 5
    columnSize:
      file.name: 335
      formula.last_edited: 316

```

---
# 🔗 Navigation Menu 🔗
- 🖇️ ***Links***
	- [[📥️ Inbox 📥️.base|📥️ Inbox 📥️]]
	- [[🎯 Projects 🎯.base|🎯 Projects 🎯]]
	- [[📔 Journals 📔.base|📔 Journal 📔]]
	- [[📝 Indexes 📝.base|📝 Indexes 📝]]
	- [[📎 Orphans 📎.base|📎 Orphans 📎]]
- ❓️ ***Help***
	- [[Tutorial]]
	- [GitHub Page](https://github.com/Hophnoph/Compendium-PKM)