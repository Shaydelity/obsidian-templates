<%*
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<sup>${sel}</sup>`;
} else {
    tR = `<sup>${tp.file.cursor()}</sup>`;
}
%>