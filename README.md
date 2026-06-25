# Course Plan — Degree Roadmap

A single-file, drag-and-drop tool for planning the courses you still need across the remaining semesters of a degree — built around real constraints: a credit-hour (CH) cap per semester and prerequisite order.

No build step, no backend, no dependencies. It's one HTML file.

## Features

- **Unscheduled tray + semester board** — add your remaining courses (code, name, credit hours, prerequisite codes), then drag them into semesters.
- **Per-semester CH cap** — set a default max CH per semester, override any individual semester (e.g. a lighter summer term), and a capacity gauge shows used/available CH, turning red if you go over.
- **Prerequisite validation** — each course shows a status dot if it's placed before a prerequisite is satisfied. If a prerequisite code isn't in your list, it's assumed already completed.
- **Auto-plan** — automatically slots your unscheduled courses into semesters in valid prerequisite order, packing each as close to its cap as it can.
- **Backups** — Export downloads a `.json` snapshot of your whole plan; Import loads one back in. Useful for moving between browsers/devices or just keeping a copy.
- **Persistence** — your plan saves automatically to your browser's local storage, so it's there next time you open the page on the same device/browser.

## Usage

Just open `index.html` in any modern browser — double-click it, or drag it into a browser tab. Nothing to install.

If this repo has GitHub Pages enabled, you can also use it directly at the Pages URL without downloading anything.

## Data & privacy

Everything you enter is stored **only in your own browser** (`localStorage`), scoped to wherever you're loading the page from. Nothing is sent to a server. That also means:

- Data doesn't sync between browsers or devices automatically — use **Export backup** / **Import backup** to move it.
- Clearing your browser's site data for this page will clear your plan too (export a backup first if that matters to you).

## License

MIT — see [LICENSE](LICENSE).
