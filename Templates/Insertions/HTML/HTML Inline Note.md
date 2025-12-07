<%*
const v = await tp.system.prompt("Inline Note (Hover Text)");
const sel = tp.file.selection();

if (sel && sel.length > 0) {
    tR = `<span class="inline-note-wrapper"><span class="inline-note-text">${sel}</span><span class="inline-note">${v}</span></span>`;
} else {
    tR = `<span class="inline-note-wrapper"><span class="inline-note-text">${tp.file.cursor()}</span><span class="inline-note">${v}</span></span>`;
}
%>