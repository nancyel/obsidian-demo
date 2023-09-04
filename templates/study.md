---
topics: 
  -
aliases: 
tags: 
creation date: <% tp.file.creation_date() %>
---

<%*  
let title = await tp.system.prompt("Set FileName")  
-%>  
<% await tp.file.move("study/" + title) %>