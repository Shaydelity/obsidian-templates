<%*
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<em>${sel}</em>`;
} else {
    tR = `<em>${tp.file.cursor()}</em>`;
}
%>
