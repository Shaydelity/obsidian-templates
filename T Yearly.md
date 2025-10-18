---
tags: [Personal/Diary]
marker: ""
title: "<% tp.file.title %>"
status: [RES]
aliases: ["<% tp.file.title %>"]
linter-yaml-title-alias: "<% tp.file.title %>"
description: ""
creation date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
modified date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
cssclasses: [daily, <% tp.date.now("dddd", 0, tp.file.title, "YYYY-MM-DD").toLowerCase() %>]
---

# <% tp.file.title %>

> [!dv-metadata-previous]
> previous:: [[<% moment(tp.file.title, "YYYY").subtract(1, "year").format("YYYY") %>]]

- - -

## Year

### Summary

- - -

> [!dv-metadata-next]
> next:: [[<% moment(tp.file.title, "YYYY").add(1, "year").format("YYYY") %>]]
