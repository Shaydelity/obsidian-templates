<%*
const v = await tp.system.prompt("Insert Link");

const openTag = `<a data-tooltip-position="top" aria-label="${v}" rel="noopener nofollow" class="external-link" href="${v}" target="_blank">`;
const closeTag = `</a>`;

tR = openTag + tp.file.cursor() + closeTag;
-%>