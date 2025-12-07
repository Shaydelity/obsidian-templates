<%*
const type = await tp.system.prompt("Callout Type");
const title = await tp.system.prompt("Callout Title");
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `> [!${type}] ${title}
> ${sel}`;
} else {
    tR = `> [!${type}] ${title}
> ${tp.file.cursor()}`;
}
%>