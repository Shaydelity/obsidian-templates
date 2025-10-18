---
tags: []
title: "<% tp.file.title.replace(/^\d{4}-\d{2}-\d{2}_/, '') %>"
status: [RES]
aliases: ["<% tp.file.title.replace(/^\d{4}-\d{2}-\d{2}_/, '') %>", "<%* let t = tp.file.title.replace(/^\d{4}-\d{2}-\d{2}_/, ''); let m = t.match(/^\s*(.*?)\s*-\s*(.+)/); if(m) tR += m[1].trim(); %>"]
linter-yaml-title-alias: "<% tp.file.title.replace(/^\d{4}-\d{2}-\d{2}_/, '') %>"
creation date & time: <% tp.file.creation_date() %>
modified date & time: <% tp.file.creation_date() %>
cssclasses: [daily, <% moment(tp.file.title, "YYYY-MM-DD").format("dddd").toLowerCase() %>]
---

# <% tp.file.title %>

- - -
## Experimental

<%*
let userInput = await tp.system.prompt("Enter text (or leave empty):");
if (userInput) {
    tR += userInput;
}
%>

<%*
let day = moment(tp.file.title, "YYYY-MM-DD").day(); // Sunday = 0, Monday = 1, ..., Saturday = 6

if (day >= 1 && day <= 5) {
    tR += `> [!anchor] Work Time
> | Time | Type | Work | Note |
> | --- | --- | --- | --- |
> | 9:30–10:00 | Indirect | Work | Note |`;
} else {
    tR += ``;
}
%>

- - -
