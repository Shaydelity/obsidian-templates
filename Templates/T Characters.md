
---
tags: []
title: "<% tp.file.title %>"
status: [RES]
aliases: ["<% tp.file.title %>"<%* let m = tp.file.title.match(/^\s*(.*?)\s*-\s*(.+)/); if(m) tR += `, "${m[1].trim()}"`; %>, <% tp.file.title.split(/\s+/).map(w => `"${w.replace(/"/g,"")}"`).slice(0,3).join(", ") %>]
linter-yaml-title-alias: "<% tp.file.title %>"
creation date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
modified date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
cssclasses: [characters, <% tp.file.title.toLowerCase()
  .replace(/['‘’]/g, "")
  .replace(/&/g, "and")
  .replace(/@/g, "at")
  .replace(/\+/g, "plus")
  .normalize("NFD").replace(/[\u0300-\u036f]/g, "") // accents
  .replace(/\s+/g, "_") // spaces → underscores
  .replace(/[^a-z0-9_-]+/g, "_") // all other invalid chars → underscores
  .replace(/^_+|_+$/g, "") %>]
---

# <% tp.file.title %>

> [!dv-metadata-top]
> up:: [[Fleeting Notes]]

- - -

##

- - -
