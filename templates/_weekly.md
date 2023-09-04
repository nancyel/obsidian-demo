---
week: <% tp.date.now("YYYY-[W]W", 0, tp.file.title, "YYYY-[W]W") %>
year: <% tp.date.now("YYYY", 0, tp.file.title, "YYYY-[W]W") %>
---

  
#### Summary
- 


#### Planning
- Open your [Calendar](https://calendar.google.com) and start planning.
- Follow your routine for weekly planning.
👉 Make sure you improve based on what you've learned this week.



#### History

<%*
Array.from(Array(7).keys()).map((i) => {
  date = tp.date.weekday("YYYY-MM-DD", i, tp.file.title, "YYYY-[W]W");
  tR += `### [[daily/${date} | ${date}]]\n`;
  tR += `![[daily/${date}#Outcomes]]\n\n`;
});
%>


#### Remaining
```dataview
TASK
FROM "daily"
WHERE file.cday > date(today) - dur(8 day)
AND !completed
SORT file.day
```

