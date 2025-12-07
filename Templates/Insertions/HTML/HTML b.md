<%*
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<b>${sel}</b>`;
} else {
    tR = `<b>${tp.file.cursor()}</b>`;
}
%>
