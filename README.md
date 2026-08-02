# IdeaSink

A tiny, private word‑processor that looks like a paper sheet of labels. Name a
label, click it, and write on its own scrollable page — with fonts, colors,
images, tables, and more. Everything is one file, works offline, and can
optionally sync between two people through GitHub.

- **One file, no install:** `IdeaSink.html` — double‑click to open in any modern browser.
- **Works on Mac and Windows** (Chrome or Edge recommended; Safari works too).
- **Your notes stay yours:** saved locally in your browser; nothing goes to any server unless you turn on GitHub sync.

---

## Quick start

1. Double‑click `IdeaSink.html`.
2. Click a blank label, type a name, press **Enter**.
3. Click the named label to open its page and start writing.
4. Use the toolbar to format; everything saves automatically.

The little version tag lives at the bottom of the **Menu** (currently **v34**).

## Multiple notebooks (name follows the file)

You can keep more than one separate IdeaSink — for example a **shared** one and a **private** local one. Each is simply a copy of `IdeaSink.html` with a **different file name**, and the name shown in the browser tab and the top‑left header **follows the file name**:

- `IdeaSink.html` → shows “IdeaSink” (this is the original/default notebook — keep your shared, GitHub‑synced one as this).
- `Private.html` → shows “Private”, `Work Ideas.html` → shows “Work Ideas”, and so on.

Each differently‑named file is a **completely separate notebook**: its own labels and pages, its own local storage, and its own Live‑sync settings. So you can have `IdeaSink.html` synced with your wife via GitHub, and `Private.html` sitting purely on your computer with sync off — they never mix, and their tabs are easy to tell apart.

A couple of notes: the name comes from the file name, so **keep a notebook’s file name stable** (renaming it starts a fresh, empty notebook under the new name — your old one is still there under the old name). If you’d rather set the name in the address bar, you can also open `IdeaSink.html?ws=AnyName`.

---

## Features

### Labels & sheets
- A home screen styled as **paper sheets of labels** (3 × 7 labels per sheet).
- **Unlimited labels** — a fresh sheet appears when one fills up; buttons below add or remove an empty sheet.
- **Name / open:** click a blank label to name it; click a named label to open its page.
- **Colors:** right‑click a label for a **64‑color palette**, plus Rename and Delete.
- **Rearrange:** drag a label onto another to reorder it.
- **Select many:** ⌘/Ctrl‑click labels (Shift‑click for a range, ⌘/Ctrl‑A for all), then move them together.
- **Sort a page** (button at the right of the tabs): Custom (drag), A–Z, Recently opened, Recently edited, or **Color (rainbow)**. Each page remembers its own choice.
- **Label lettering:** Menu → “Label font…” sets the font used on labels and tabs.

### Main pages (the tabs on top)
- Each tab is a separate **main page** with its own labels — keep different topics apart.
- **Two kinds of page:** a **sheet of labels** (the usual) or a **single writing page** (marked ▤) that opens straight into one page.
- Right‑click a tab to switch its type, recolor, rename, make it **local**, or delete it; drag tabs to reorder.
- Tabs **wrap onto a second row** when one row fills up.
- **Move labels between pages:** drag a label (or a multi‑selection) onto a tab, or right‑click → “Move to …”.
- **Local (private) pages:** right‑click a tab → **“Make local (this device only)”**. A local page shows in **bold italic with a 🔒** and **never syncs to GitHub** — it stays only on this computer, even while your other tabs sync with your wife. Turning a page local (or moving a label into one) removes its labels from the shared repo so others no longer see them, while your copy stays put. Right‑click → “Make shared” to start syncing it again. (This only matters when Live sync is on; the tab uses Arial like the rest.)

### Writing (the editor)
- **Fonts:** 10 choices (Arial is the default) — Menu also lets you set the label font separately.
- **Size** and **line spacing** (Single … Double) — line spacing applies to the paragraphs you select.
- **Page view** (the Continuous / Pages dropdown): keep a page as one long **Continuous** sheet, or **split it into separate page cards** (Letter or A4) that look and print like Microsoft Word’s Print Layout. Each sheet remembers its own choice, and the last choice becomes the default for new sheets. Printing and Save‑as‑PDF produce real separate pages either way.
- **Page numbers**: optional, and chosen right next to the page‑view control in the toolbar. When a sheet is set to “Pages”, a second dropdown appears — **No page #**, **Page # · center**, or **Page # · right**. It’s remembered per sheet, and your last choice becomes the default for new sheets. Page numbers are baked into **PDF** and **Word** exports too (Word gets a live, auto‑updating page number).
- **Print** (the printer button in the toolbar, or **⌘/Ctrl‑P**): opens your computer’s print dialog, which lists all of your installed printers (and “Save as PDF”) — just pick one. What prints matches the page view you chose: “Pages” sheets print as real Letter/A4 pages with your page numbers. You can also print a label’s page straight from the sheet by right‑clicking it → **Save or print → Print / PDF…**.
- **Bold, Italic, Underline, Strikethrough.**
- **Text color** (24) and **Highlight** (8 colors + “no highlight”).
- **Bulleted and numbered lists** — Tab / Shift‑Tab to indent, Enter on an empty bullet to leave the list.
- **Hyperlinks:** select text → right‑click → Add hyperlink (⌘/Ctrl‑click a link to open it).
- **Undo / Redo:** the ↶ ↷ buttons, or ⌘Z / ⌘⇧Z.
- **Paste matches your page:** pasted text takes on the page’s font instead of the copied font (bold, italic, lists, and links are kept).

### Your name & comments (great with live sync)
- **Menu → “Your name…”** sets the name shown on your comments (and to the other person while live sync is on).
- **Comment on any text:** select some words, then click the 💬 button in the toolbar (or right‑click → “Add comment…”). The text gets a soft highlight and a little 💬 marker.
- **Read & reply:** click the 💬 marker to open the note, add replies back and forth, then **Resolve** it (or **Reopen** / **Delete**). Perfect for you and your wife to talk over each other’s ideas.
- Deleting the highlighted text automatically clears its comment.

### Saving a page as a file
- **In a page:** the ⬇ button (top‑right of the toolbar) saves the current page.
- **From the sheet:** right‑click a label → **“Save as (Word / text / PDF)…”**.
- Choose **Word** (`.doc`, opens in Microsoft Word), **Plain text** (`.txt`), or **PDF** (opens the print dialog — pick “Save as PDF”). Comment markers are left out of the exported file.

### Images
- **Paste, drag in, or insert** an image; it’s kept at full resolution.
- **Pixel‑perfect display** (never blurrily upscaled); drag an image’s corner to resize.
- **Double‑click** an image for a full‑size zoom view; right‑click for width presets, “View full size”, and **Image info** (shows exactly how many pixels a copy contains).

### PDFs (sharp)
- **Drag a PDF file onto a page** and its pages are rendered as **high‑resolution, sharp** images — much crisper than copy‑pasting from a PDF viewer. For multi‑page PDFs you choose which pages to insert.

### Tables
- Insert an **n × n** table from a grid picker.
- **Drag cell borders** to resize columns and rows; **right‑click** inside a table to add/delete rows and columns; **Tab** moves between cells.

### Saving & backups
- **Autosaves** continuously in your browser (per browser, so stick with one).
- **Menu → “Back up notes”** downloads a single JSON file of everything; **“Restore backup”** loads one back (it *merges*, keeping the newer version of each label).
- **Menu → “Automatic backup…”** writes a single `IdeaSink-autobackup.json` into a folder you choose (e.g. this IdeaSink folder) every few minutes, only when something changed. An optional checkbox also keeps one dated copy per day.

### Live sync & sharing (optional — see setup below)
- **Menu → “Live sync (GitHub)…”** stores the notebook in a GitHub repository you both use, so two people share the same notes (syncing every few seconds) and **see each other’s name** at the top while both are in it.

---

## Keyboard shortcuts

| Action | Shortcut |
| --- | --- |
| Bold / Italic / Underline | ⌘B / ⌘I / ⌘U |
| Undo / Redo | ⌘Z / ⌘⇧Z |
| Indent / outdent a list item | Tab / Shift‑Tab |
| Leave a list | Enter on an empty bullet |
| Open a link | ⌘‑click the link |
| Move between table cells | Tab |

(On Windows use **Ctrl** instead of ⌘.)

---

## Live sync setup (GitHub)

This lets two people share one notebook. It’s a one‑time setup of about ten
minutes. One person (the owner) does Parts 1–3; the other does Part 4.

### Part 1 — Create the private repository
1. Go to **github.com** and sign in (create a free account if needed).
2. Click the **+** in the top‑right corner → **New repository**.
3. **Repository name:** `ideasink-notes` (any name works — remember it).
4. Choose **Private**.
5. Check **Add a README file** (this initializes the repo so IdeaSink can write to it).
6. Click **Create repository**.

### Part 2 — Create the access token
1. Click your profile picture (top‑right) → **Settings**.
2. In the left sidebar, scroll down and click **Developer settings**.
3. Click **Personal access tokens** → **Fine‑grained tokens**.
4. Click **Generate new token**.
5. **Token name:** `IdeaSink`. **Expiration:** pick a long one (e.g. 1 year — note when to renew). **Resource owner:** your own account.
6. Under **Repository access**, choose **Only select repositories** and select `ideasink-notes`. (Do this *before* the next step — permissions won’t apply until a repository is chosen.)
7. Scroll to **Permissions → Repository permissions** and click **Add permissions**. In the box that appears, type **Contents** and select it. A small access dropdown then shows up next to **Contents** — set it to **Read and write**. (Heads‑up: the “Read and write” option only appears *after* you add Contents this way. Contents is the only permission needed.)
8. Click **Generate token** and **copy** it — it starts with `github_pat_…` and is shown only once.

> **Simpler alternative if that screen gives you trouble:** make a **classic** token instead — go to **Developer settings → Personal access tokens → Tokens (classic) → Generate new token (classic)**, name it, set an expiration, tick the single top‑level **`repo`** checkbox, and generate. It works identically in IdeaSink. The only trade‑off is that a classic `repo` token can reach all of your repositories, so keep it private and set an expiration.

### Part 3 — Turn on sync in IdeaSink
1. Open IdeaSink → Menu → **Live sync (GitHub)…**.
2. **Your name:** e.g. `Larry`. **Repository:** `yourusername/ideasink-notes`. **Token:** paste the `github_pat_…`.
3. Click **Connect**. The dot by the Menu turns green; IdeaSink creates the data file automatically.

### Part 4 — Set up the second person
The simplest route for a couple is to **share that same token** (it’s just the
key to this one private repo, and each person still shows their own name):
- Send them `IdeaSink.html` (if they don’t have it), the repo name `yourusername/ideasink-notes`, and the token.
- They open IdeaSink → Menu → **Live sync (GitHub)…**, enter **their** name, the same repo, and the same token, then click **Connect**.

Prefer separate, independently‑revocable tokens? Put the repo in a free GitHub
**organization**, add both people as members, and each creates a token on the
org. (Ask if you want those steps.)

### Notes on sync
- **Near‑live:** it syncs every few seconds (not instant like Google Docs). If both people edit the *same* label at the same moment, the later save wins.
- **Deletions and edits** both sync; different labels edited at once merge cleanly.
- The token is a password to the repo — **share it privately**, and regenerate it when it expires.
- **Version history for free:** every save is a commit, so you can see past versions in the repo.
- **One file per label:** each label is stored as its own small file in a `notes/` folder, alongside a tiny `index.json` for the tabs and deletions. This means the notebook can hold **lots of images without hitting size limits** (GitHub allows up to 100 MB *per file*, so only a single label stuffed with images could ever be a concern — IdeaSink warns you if one gets close). It also makes syncing **faster and calmer**: saving one label only re-uploads that one file, and you and your wife editing *different* labels never collide.
- **Both people need v31 or newer.** The storage layout changed to per‑label files in v31. The first time you connect, IdeaSink automatically migrates an older single‑file notebook — but the other person must also be on v31+ or they’ll stop seeing updates. Just send them the new `IdeaSink.html`.
- Even if a sync ever fails, **nothing is lost** — everything is always kept on your own device first.
- **Works for a group, not just two.** Everyone points at the same repo; edits to different labels merge cleanly and the top strip shows everyone currently in it by name. Built to scale: idle checks use conditional requests (so they’re free and don’t eat GitHub’s hourly limit), each person has their own tiny presence file (no collisions), and old deletion records are pruned automatically. For more than two people, give **each person their own token** (add them to the repo, or use a GitHub organization) rather than sharing one — that way each gets their own hourly quota.

---

## Where your data lives
- Normally: inside your browser on this computer (per browser). Back up now and then.
- With Automatic backup on: also as a JSON file in your chosen folder.
- With Live sync on: also in your GitHub repository (private).

## Good to know
- Use the **same browser** on a given computer, or your notes will look missing (each browser keeps its own copy). Sync or a restored backup brings them together.
- Keep only one copy of `IdeaSink.html` in your folder to avoid opening an old version by mistake; the Menu shows the version number so you can confirm.

*IdeaSink v34*
