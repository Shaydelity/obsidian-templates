
---
tags: [Personal/Diary]
marker: ""
title: <% tp.file.title %>
status: [RES]
aliases: ["<% tp.file.title %>"]
linter-yaml-title-alias: "<% tp.file.title %>"
description: ""
creation date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
modified date & time: <%tp.date.now("YYYY-MM-DD")%> <%tp.date.now("HH:mm")%>
cssclasses: [weekly, <% moment(tp.file.title, "GGGG-[W]WW").format("[cw]ww").toLowerCase() %>]
---

# <% tp.file.title %>

> [!dv-metadata-top]
> year:: [[<% moment(tp.file.title, "GGGG-[W]WW").format("YYYY") %>]]
> 
> month:: [[<% moment(tp.file.title, "GGGG-[W]WW").format("YYYY-MM") %>]]

> [!dv-metadata-previous]
> previous:: [[<% moment(tp.file.title, "GGGG-[W]WW").subtract(1, "week").format("GGGG-[W]WW") %>]]

- - -

## My Affairs - <% moment(tp.file.title, "GGGG-[W]WW").format("[CW]WW, YYYY") %>

[[<% moment(tp.file.title, "GGGG-[W]WW").format("GGGG-[W]WW") %>|This week]]

![[<% moment(tp.file.title, "GGGG-[W]WW").format("YYYY-MM") %>#^Monthly]]

> [!anchor] Concrete Affairs
>
> - [ ] Finish [[<% moment(tp.file.title, "GGGG-[W]WW").subtract(1, "week").format("GGGG-[W]WW") %>]]
> - [ ] ! Monthly Payments
^concrete-affairs

> [!anchor] Additional Affairs
>
> - [ ] B
^additional-affairs

> [!anchor] Work Affairs
>
> - Zeiterfassung
> - ~~Ticket Moving~~
> - [ ] B
^work-affairs

## Week

- - -

> [!dv-metadata-next]
> next:: [[<% moment(tp.file.title, "GGGG-[W]WW").add(1, "week").format("GGGG-[W]WW") %>]]
