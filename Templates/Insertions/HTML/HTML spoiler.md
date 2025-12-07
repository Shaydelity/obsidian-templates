<%*
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<span class="spoiler">${sel}</span>`;
} else {
    tR = `<span class="spoiler">${tp.file.cursor()}</span>`;
}
%>