<%*
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<u>${sel}</u>`;
} else {
    tR = `<u>${tp.file.cursor()}</u>`;
}
%>