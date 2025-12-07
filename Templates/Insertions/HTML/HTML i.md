<%*
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<i>${sel}</i>`;
} else {
    tR = `<i>${tp.file.cursor()}</i>`;
}
%>
