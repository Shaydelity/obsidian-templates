
---
tags: [Personal/Diary]
marker: ""
title: <% tp.file.title %>
status: [RES]
aliases: ["<% tp.file.title %>"]
linter-yaml-title-alias: "<% tp.file.title %>"
creation date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
modified date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
cssclasses: [MoC]
---

# <% tp.file.title %>

> [!dv-metadata-top]
> year:: [[<% moment(tp.file.title, "YYYY-MM").format("YYYY") %>]]

> [!dv-metadata-previous]
> previous:: [[<% moment(tp.file.title, "YYYY-MM").subtract(1, "month").format("YYYY-MM") %>]]

- - -

## Month

> [!anchor] Abstract Goals - <% moment(tp.file.title, "YYYY-MM").format("MMMM, YYYY") %>
>
> [[<% moment(tp.file.title, "YYYY-MM").format("YYYY-MM") %>|This month]]
>
> 1. ?
^monthly

### Summary

- - -

> [!dv-metadata-next]
> next:: [[<% moment(tp.file.title, "YYYY-MM").add(1, "month").format("YYYY-MM") %>]]
