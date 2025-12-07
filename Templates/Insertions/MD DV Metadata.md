<%*
const type = await tp.system.prompt("Type (\"-top\", \"-previous\", \"-next\")");
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `> [!dv-metadata${type}]
> ${sel}`;
} else {
    tR = `> [!dv-metadata${type}]
> ${tp.file.cursor()}`;
}
%>