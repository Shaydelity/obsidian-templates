# Shaydelity's Obsidian Templates

These are the templates I use regularly within [my obsidian vault](https://github.com/Shaydelity/.obsidian). I share them so that others may be able to take things from them for their own vaults and needs.

## Structure

> You may notice that I put a clear line before the frontmatter! This is **INTENTIONAL** because when you use the template the YAML frontmatter will be reformatted in a format that I *do not want*. That is unless you make sure it is **not** recognized as frontmatter once the template's generation finished. That is what I have the clear line for, which I immediately remove (manually) after the file's generation.

1. Excalidraw: Folder of Templates for [Excalidraw](https://github.com/zsviczian/obsidian-excalidraw-plugin) (I have not yet made any, dunno if that will change).
2. Insertions: Folder of Templates meant to be inserted during the making of a document. These templates are meant to be used with the `Templater: Open Insert Template Modal` hotkey (standard on `ALT + E`, in [my .obsidian files](https://github.com/Shaydelity/.obsidian) `ALT + T`). Contains lists of contents for (german) analysis writing and HTML/Markdown insertion templates. 
    1. HTML: These Tempaltes are meant to make it more comfortable, efficient, and faster to use HTML when typing. **Make sure to have automatic cursor jumping enabled in the templater settings!**
    2. MD: These templates are used for markdown callouts. The special ones only have CSS featured in the [Noctus Theme](https://github.com/Reparse-dev/noctus-obsidian-theme) or (yet to be relased) snippets related to it.
3. Kanban: Meant for kanban notes. I recommend having a hotkey or quick access to the "switch to kanban view" command. Make sure that if you use a [linter](https://github.com/platers/obsidian-linter) or similar that it won't mess too much with the file/best disable it completely by adding a regex (`\b[Kk]anban\b`) for example that track the file name (anything that includes "kanban" or "Kanban").
4. The common templates: Each template is designed to be used within certain folders, after which they are also named. They are not supposed to be manually invoked. I use the [Advanced New File](https://github.com/vanadium23/obsidian-advanced-new-file) plugin to always create files in the folders they are supposed to end up in, making all templating wholly automatic. They always start with a "T" for template which makes sure there won't occur any double file names within my vault. 

> The "T Note" template is the standard one used if none other is defined. The Anchor of Content template is not yet used and mostly a filler.

## Snippet for HTML Insertions

Here is some CSS that is needed for the "Inline Note" and "Spoiler" insertions with some minor added styling for the quote tag (`q`).
***Most of this CSS is just a temporary way to go about all this, the end goal is full integration of these things in the [Noctus Theme](https://github.com/Reparse-dev/noctus-obsidian-theme), which will have a heavy rewrite soon.***

To use it, just make a text file, paste this code into it, and change its file extension from `.txt` to `.css`. Finally just place it in the `.obsidian/snippets` folder and enable it in the Obsidian settings (`Settings > Appearance > Snippets`).

```
abbr, span.inline-note-text {
  position: relative;
  cursor: help;
  border-bottom: 1px dotted #FFF;
  cursor: text !important;
}

span.inline-note-text {
    border-bottom: 1px dotted #888;
}

body:has(span.inline-note-text:hover) .tooltip {
  display: none;
}

span.inline-note-wrapper {
  position: relative;
  display: inline-block;
/*   margin-left: 0.3em; Only needed when used with the Noctus Theme*/
/*   p > & { */
/*     margin-left: 0em; */
/*   } */
}

span.inline-note-text {
  cursor: pointer;
}

span.inline-note {
  box-shadow: 0 2px 8px var(--background-modifier-box-shadow);
  background-color: var(--background-modifier-message);
  border-radius: var(--radius-s);
  color: #FAFAFA;
  font-size: var(--font-ui-smaller);
  font-weight: var(--font-medium);
  display: none;
  position: absolute;
  bottom: 100%;
  left: 50%;
  transform: translateX(-50%);
  padding: var(--size-4-1) var(--size-4-2);
  border-radius: 4px;
  max-width: 30em;
  max-height: 10em;
  line-height: var(--line-height-tight);
  z-index: var(--layer-tooltip);
  white-space: pre-wrap;
  overflow-y: scroll;
  scroll-snap-align: start;
}

span.inline-note-wrapper:hover span.inline-note,
span.inline-note:hover {
  display: block;
}

span.spoiler {
  color: black;
  background-color: black;
  padding: 4px;
  border-radius: 5px;
}

span.spoiler:hover {
  color: white;
  background-color: black;
}

q {
  background-color: rgba(150,150,150,0.2);
}
```
