---
tags: [Personal/Diary]
marker: ""
title: "<% tp.file.title %>"
status: []
aliases: ["<% tp.file.title %>"]
description: ""
creation date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
modified date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
cssclasses: [daily, <% moment(tp.file.title, "YYYY-MM-DD").format("dddd").toLowerCase() %>]
---

# <% tp.file.title %>

> [!dv-metadata-top]
> year:: [[<% moment(tp.file.title, "YYYY-MM-DD").format("YYYY") %>]]
> 
> month:: [[<% moment(tp.file.title, "YYYY-MM-DD").format("YYYY-MM") %>]]
> 
> week:: [[<% moment(tp.file.title, "YYYY-MM-DD").format("GGGG-[W]WW") %>]]

> [!dv-metadata-previous]
> previous:: [[<% moment(tp.file.title, "YYYY-MM-DD").subtract(1, "day").format("YYYY-MM-DD") %>]]

- - -

| Time       | Type     | Work                         |
| ---------- | -------- | ---------------------------- |
| 9:30–10:00 | Indirect |  |
|            |          |                              |

![[<% moment(tp.file.title, "YYYY-MM-DD").format("GGGG-[W]WW") %>#My Affairs - CW42, 2025]]

- - -

> [!dv-metadata-next]
> next:: [[<% moment(tp.file.title, "YYYY-MM-DD").add(1, "day").format("YYYY-MM-DD") %>]]
