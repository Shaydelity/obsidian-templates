<%*
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<small>${sel}</small>`;
} else {
    tR = `<small>${tp.file.cursor()}</small>`;
}
%>