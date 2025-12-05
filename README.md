# Shaydelity's Obsidian Templates

These are the templates I use regularly within [my obsidian vault](https://github.com/Shaydelity/.obsidian). I share them so that others may be able to take things from them for their own vaults and needs.

## Structure

> You may notice that I put a clear line before the frontmatter! This is **INTENTIONAL** because when you use the template the YAML frontmatter will be reformatted in a format that I *do not want*. That is unless you make sure it is **not** recognized as frontmatter once the template's generation finished. That is what I have the clear line for, which I immediately remove (manually) after the file's generation.

1. Excalidraw: Folder of Templates for [Excalidraw](https://github.com/zsviczian/obsidian-excalidraw-plugin) (I have not yet made any, dunno if that will change).
2. Insertions: Folder of Templates meant to be inserted during the making of a document. Only has lists of contents for (german) analysis writing and similar from my school days currently.
    1. HTML: These templates are meant to be used with the `Templater: Open Insert Template Modal` hotkey (standard on `ALT + E`, in [my .obsidian files](https://github.com/Shaydelity/.obsidian) `ALT + T`) and are meant to make it more comfortable, efficient, and faster to use HTML when typing. *Still recommend using it sparingly though as using HTML kinda goes against the idea of using Markdown to begin with.*
3. Kanban: Meant for kanban notes. I recommend having a hotkey or quick access to the "switch to kanban view" command. Make sure that if you use a [linter](https://github.com/platers/obsidian-linter) or similar that it won't mess too much with the file/best disable it completely by adding a regex (`\b[Kk]anban\b`) for example that track the file name (anything that includes "kanban" or "Kanban").
4. The common templates: Each template is designed to be used within certain folders, after which they are also named. They are not supposed to be manually invoked. I use the [Advanced New File](https://github.com/vanadium23/obsidian-advanced-new-file) plugin to always create files in the folders they are supposed to end up in, making all templating wholly automatic. They always start with a "T" for template which makes sure there won't occur any double file names within my vault. 

> The "T Note" template is the standard one used if none other is defined. The Anchor of Content template is not yet used and mostly a filler.
