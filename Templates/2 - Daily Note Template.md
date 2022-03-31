---
creation date: <% tp.file.creation_date() %>
modification date: <% tp.file.last_modified_date("dddd Do MMMM YYYY HH:mm:ss") %>
tags: ['daily_note']
---

<<[[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD" ) %>]]|[[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD" ) %>]]>>

# <% tp.file.title %>

<% tp.web.daily_quote() %>

## Habits & Todo's
```todoist
{
"name": "Today's Tasks",
"filter": "(today|overdue) & #Personal",
"sorting": ["priority"]
}
```


## Workbench

<% tp.file.cursor(1) %>


## Reflection


--- 
[Related work note (if created)](obsidian://open?vault=Work%20Brain&file=Files%2F<% tp.date.now("YYYY-MM-DD", 0) %>)