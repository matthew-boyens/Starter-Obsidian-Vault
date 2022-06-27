---
creation date: <% tp.file.creation_date() %>
modification date: <% tp.file.last_modified_date("dddd Do MMMM YYYY HH:mm:ss") %>
tags: ['daily_note']
---

<<[[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD" ) %>]]|[[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD" ) %>]]>>

# <% tp.file.title %>

<%*
    try {
        tR+= await tp.web.daily_quote()
    } catch (err) {
        new Notice("Error: \n" + err , 2000);
    }
%>

## Habits & Todo's

### Due
```tasks
not done
due before tomorrow
```

## Workbench

<% tp.file.cursor(1) %>





## Prayer points 
```tasks
not done
exclude sub-items
heading includes pray
```
```tasks
not done
exclude sub-items
description includes pray
```

## Completed Today
```tasks
done today

```

## Reflection






---
## Upcoming
### Happening in the next few weeks
```tasks
not done
happens before in two weeks
exclude sub-items
description does not include pray
heading does not include pray
```
---
### Not booked in 
## Unscoped Tasks (missing date/priority)
```tasks
no due date
no start date
no scheduled date
not done
exclude sub-items
heading does not include pray
description does not include pray
group by heading
```



--- 
[Related work note (if created)](obsidian://open?vault=Work%20Brain&file=Files%2F<% tp.date.now("YYYY-MM-DD", 0) %>)