# ITMC Study Vault — Quick Start

A shared-friendly Obsidian vault for the M.Sc. IT-Management & -Consulting (ITMC) at Universität Hamburg. Start here, then use the [[Semester 1 Overview]] to navigate the courses.

## First-time setup

1. Open this folder as a vault in Obsidian (**Open folder as vault**).
2. Go to **Settings → Core plugins** and enable **Templates** and **Command palette**.
3. Go to **Settings → Core plugins → Templates** and set **Template folder location** to `Templates`.
4. Optional: go to **Settings → Hotkeys**, search for **Templates: Insert template**, and assign a shortcut you like. Suggested: `Ctrl+Alt+T` (Windows/Linux) or `Cmd+Option+T` (macOS). The shortcut is your preference; use the command palette if you don't assign one.
5. In **Settings → Editor**, set **Default location for new notes** to **Same folder as current file** (or your preferred location). You can create notes directly inside a course subfolder from the File explorer.

> Template placeholders such as `{{title}}` and `{{date}}` are filled when you insert a template. The course field is intentionally left blank for you to fill in.

## Everyday shortcuts

| Action | Shortcut / command |
|---|---|
| Open command palette | `Ctrl+P` (Windows/Linux) or `Cmd+P` (macOS) |
| Insert a template | Command palette → search `Templates: Insert template`; or use the custom hotkey you assigned |
| Find and open a note by name | Command palette → `Quick switcher: Open quick switcher` (assign a hotkey under **Settings → Hotkeys** if you use it often) |
| Search vault contents | Command palette → search `Search: Search in all files` |
| Create a note | Click **New note** in the ribbon or use the command palette → `Create new note` |

Shortcut assignments can vary by operating system and vault settings. Search for a command in **Settings → Hotkeys** to see or change its binding.

## Make a course note from a template

1. Open the course page from [[Semester 1 Overview]].
2. Create a note in that course's `Notes` folder (for example, `Semester 1/Value & Service in an AI-driven World/Notes/Session 1`).
3. With the new note open, put the cursor where you want the template content.
4. Run **Templates: Insert template** from the command palette, or use your assigned template shortcut. Choose **Lecture Note**, **Reading Note**, **Meeting Note**, or **Exam Revision**.
5. Fill in the course, date, and other blank fields. Add links to related course pages with `[[Course title]]`.

Templates: [[Templates/Lecture Note]], [[Templates/Reading Note]], [[Templates/Meeting Note]], and [[Templates/Exam Revision]]. Course pages and their `Notes`, `Material`, and `Exam Prep` folders are under `Semester 1/`.

## Keep the vault tidy

- Use one course folder per module; keep class notes in its `Notes` folder.
- Put your own summaries and links in notes. Keep downloaded files in `Material` and link to them from the relevant course page.
- Use descriptive filenames, such as `2026-10-16 — EP Kickoff` or `Service lifecycle — concept`.
- Update the [[Semester 1 Overview]] if you add courses or confirm timetable details.
- Check STiNE for current dates, registration, and rooms; the linked UHH timetable can change.

## Prepare this folder for GitHub

This vault has a root `.gitignore` for IDE files, transient Obsidian state, and installed community-plugin files. Core vault settings and Markdown notes remain shareable. Before the first push:

1. Review every note and file; remove personal data and anything you do not have permission to publish.
2. Check that `Material/` contains only files you intend and are allowed to share. Prefer linking to course sources over committing restricted lecture slides or recordings.
3. Create an empty repository on GitHub. If you want others to browse the notes, choose public; otherwise choose private.
4. In a terminal opened in this vault folder, run:

   ```powershell
   git init
   git add .
   git status
   git commit -m "Initialize ITMC study vault"
   git branch -M main
   git remote add origin https://github.com/USERNAME/REPOSITORY.git
   git push -u origin main
   ```

   Replace `USERNAME/REPOSITORY` with your GitHub account and repository name. If this folder is already a Git repository, skip `git init` and inspect `git status` before adding files.
5. For future updates, review `git status`, then `git add`, `git commit`, and `git push` as needed.

If other people will clone the vault, tell them to enable the **Templates** core plugin and set the template folder to `Templates` (see **First-time setup**).

## Useful links

- [[Semester 1 Overview]]
- [UHH ITMC teaching overview](https://www.inf.uni-hamburg.de/studies/master/itmc/landing/lehre.html)
- [UHH ITMC study plans](https://www.inf.uni-hamburg.de/studies/master/itmc/course-catalogue.html)
- [Obsidian Templates help](https://help.obsidian.md/Plugins/Templates)
- [Obsidian Command palette help](https://help.obsidian.md/Plugins/Command%2Bpalette)

