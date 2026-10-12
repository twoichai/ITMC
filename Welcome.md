# ITMC Study Vault — Quick Start

A shared-friendly Obsidian vault for the M.Sc. IT-Management & -Consulting (ITMC) at Universität Hamburg. Start with the [[Semester 1 Overview]] for courses and [[Study Method]] for the evidence-informed study workflow.

## First-time setup

1. Open this folder as a vault in Obsidian (**Open folder as vault**).
2. Enable the **Command palette** core plugin in **Settings → Core plugins**.
3. Install and enable the community plugin **Templater**: **Settings → Community plugins → Browse**, search “Templater,” install, then enable it.
4. In **Settings → Templater**, set **Template folder location** to `Templates`.
5. Optional: in **Settings → Hotkeys**, search for **Templater: Open insert template modal** and assign a shortcut, such as `Ctrl+Alt+T` (Windows/Linux) or `Cmd+Option+T` (macOS). You can also run it from the command palette.
6. Create notes inside the course's `Notes` folder using the File explorer. In **Settings → Editor**, set **Default location for new notes** to **Same folder as current file** if that suits your workflow.

> Templater derives the course link from the note's folder and fills the title and date. This assumes notes are stored under `Semester 1/<course>/...`.

## Everyday shortcuts

| Action | Shortcut / command |
|---|---|
| Open command palette | `Ctrl+P` (Windows/Linux) or `Cmd+P` (macOS) |
| Insert a template | **Templater: Open insert template modal**, or your custom hotkey |
| Find a note | Command palette → `Quick switcher: Open quick switcher` |
| Search vault | Command palette → `Search: Search in all files` |
| Create a note | **New note** in the ribbon, then move it into the course `Notes` folder if needed |

## Make a course note

1. Open the course from [[Semester 1 Overview]].
2. Create and name a note in that course's `Notes` folder (for example, `Session 1`).
3. Run **Templater: Open insert template modal** and choose **Lecture Note**, **Reading Note**, **Meeting Note**, or **Exam Revision**.
4. Templater fills the course link, title, and date where included. The templates prompt you to capture ideas selectively, explain them from memory, check and correct gaps, and revisit important material over time. See [[Study Method]].

**Do not use Obsidian's separate `Templates: Insert template` command** for these files; it inserts Templater code as plain text.

### If `<% ... %>` code appears literally

Keep the note open, open the command palette, and run **Templater: Replace templates in the active file**. For future notes, use **Templater: Open insert template modal**. If either Templater command is missing, check that the community plugin is installed and enabled.

Templates: [[Templates/Lecture Note]], [[Templates/Reading Note]], [[Templates/Meeting Note]], and [[Templates/Exam Revision]]. Course folders are under `Semester 1/`, each with `Notes`, `Material`, and `Exam Prep` subfolders.

## Keep the vault useful

- Capture your own summaries and links in notes; put permitted source files in `Material`.
- Use a clear filename, such as `Session 1` or `Service lifecycle — concept`.
- For lecture and reading notes, do a short closed-source recall before rereading. Correct gaps and turn them into questions.
- Revisit important questions on separate days; spend more time on missed or uncertain items.
- Check STiNE for current dates, registration, and rooms.

## GitHub

The root `.gitignore` excludes IDE files, transient Obsidian state, and installed community-plugin files. Before pushing, review notes for personal data and check that `Material/` contains only files you are allowed to share. Use `git status` to review changes, then `git add`, `git commit`, and `git push` as needed.

People cloning the vault need to install and enable Templater and set its template folder to `Templates`; community plugins are not bundled in this repository.

## Links

- [[Semester 1 Overview]]
- [[Study Method]]
- [UHH ITMC teaching overview](https://www.inf.uni-hamburg.de/studies/master/itmc/landing/lehre.html)
- [UHH ITMC study plans](https://www.inf.uni-hamburg.de/studies/master/itmc/course-catalogue.html)
- [Templater documentation](https://silentvoid13.github.io/Templater/)
- [Obsidian Command palette help](https://help.obsidian.md/Plugins/Command%2Bpalette)
