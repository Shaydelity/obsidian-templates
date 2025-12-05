
---
tags: []
title: "<% tp.file.title.replace(/^\d{4}-\d{2}-\d{2}_/, '') %>"
status: [RES]
aliases: ["<% tp.file.title.replace(/^\d{4}-\d{2}-\d{2}_/, '') %>"<%* let t = tp.file.title.replace(/^\d{4}-\d{2}-\d{2}_/, ''); let m = t.match(/^\s*(.*?)\s*-\s*(.+)/); if(m) tR += `, "${m[1].trim()}"`; %>]
linter-yaml-title-alias: "<% tp.file.title.replace(/^\d{4}-\d{2}-\d{2}_/, '') %>"
creation date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
modified date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
cssclasses: [scenes]
---

# <% tp.file.title %>

> [!dv-metadata-top]
> up:: [[Scenes]]

- - -

##


- - -