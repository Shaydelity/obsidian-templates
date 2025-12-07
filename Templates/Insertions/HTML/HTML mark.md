<%*
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<mark>${sel}</mark>`;
} else {
    tR = `<mark>${tp.file.cursor()}</mark>`;
}
%>