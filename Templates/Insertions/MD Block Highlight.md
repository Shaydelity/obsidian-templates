<%*
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `> [!highlight]
> ${sel}
^highlight`;
} else {
    tR = `> [!highlight]
> ${tp.file.cursor()}
^highlight`;
}
%>