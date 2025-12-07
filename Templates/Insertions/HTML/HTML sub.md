<%*
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<sub>${sel}</sub>`;
} else {
    tR = `<sub>${tp.file.cursor()}</sub>`;
}
%>