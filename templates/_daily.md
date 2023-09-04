---
date: <% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-MM-DD") %>
week: <% tp.date.now("YYYY-[W]W", 0, tp.file.title, "YYYY-MM-DD") %>
year: <% tp.date.now("YYYY", 0, tp.file.title, "YYYY-MM-DD") %>
---

#### Work
- [ ] 

#### Meetings
- 

#### Outcomes
1. 


### Files Created Today
```dataview
list file.ctime
where file.ctime > this.file.day and file.ctime < (this.file.day + dur(1 day))
```

### Files Modified Today
```dataview
list file.mtime
where file.mtime > this.file.day and file.mtime < (this.file.day + dur(1 day))
```