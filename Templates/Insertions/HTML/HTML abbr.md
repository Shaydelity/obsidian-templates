<%*
const v = await tp.system.prompt("Hover Text");
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<abbr class="abbreviation" aria-label="${v}" data-title="${v}" title="${v}">${sel}</abbr>`;
} else {
    tR = `<abbr class="abbreviation" aria-label="${v}" data-title="${v}" title="${v}">${tp.file.cursor()}</abbr>`;
}
%>