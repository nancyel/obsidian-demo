---
creation date: <% tp.file.creation_date("YYYY-MM-DD HH:mm:ss") %>
alias:
---
#temp

<%*  
let title = await tp.system.prompt("Set FileName")  
-%>  
<% await tp.file.move("temporary/" + title) %>
