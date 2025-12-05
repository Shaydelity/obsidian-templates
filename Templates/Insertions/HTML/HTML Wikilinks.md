<%*
const v = await tp.system.prompt("Note to link to (No Aliases)");

const openTag = `<a data-tooltip-position="top" aria-label="${v}" data-href="${v}" href="${v}" class="internal-link" target="_blank" rel="noopener nofollow">`;
const closeTag = `</a>`;

tR = openTag + tp.file.cursor() + closeTag;
-%>