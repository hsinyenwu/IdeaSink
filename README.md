# IdeaSink

A tiny, private word‑processor that looks like a paper sheet of labels. Name a
label, click it, and write on its own scrollable page — with fonts, colors,
images, tables, and more. Everything is one file, works offline, and can
optionally sync between two people through GitHub.

- **One file, no install:** `IdeaSink.html` — double‑click to open in any modern browser.
- **Works on Mac and Windows** (Chrome or Edge recommended; Safari works too).
- **Your notes stay yours:** saved locally in your browser; nothing goes to any server unless you turn on GitHub sync. (Because they live *in the browser*, pick a backup folder early — see “Saving & backups”.)

---

## Quick start

1. Double‑click `IdeaSink.html`.
2. Click a blank label, type a name, press **Enter**.
3. Click the named label to open its page and start writing.
4. Use the toolbar to format; everything saves automatically.
5. **Set a backup folder** the first time you are asked — **Menu → “Automatic backup…” → “Choose backup folder…”**. Until you do, your notes exist only inside the browser and clearing browsing data would delete them. See “Saving & backups” below.

The little version tag lives at the bottom of the **Menu** (currently **v50**).

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
- Right‑click a tab to switch its type, recolor, rename, make it **private**, or delete it; drag tabs to reorder.
- Tabs **wrap onto a second row** when one row fills up.
- **Move labels between pages:** drag a label (or a multi‑selection) onto a tab, or right‑click → “Move to …”.
- **Private pages (only you):** right‑click a tab → **“Make private (only you)”**. A private page shows in **bold italic with a 🔒**. It **still backs up to GitHub**, but into *your own* area of the repo (`private/<your‑id>.json`) that **other people’s IdeaSink never reads** — so it’s preserved and available if you reinstall, yet your wife’s IdeaSink won’t show it. Turning a page private (or moving a label into one) also removes its labels from the shared copy so others stop seeing them. Right‑click → “Make shared” to put it back in the shared notebook.
- **Password‑protect private pages:** Menu → **“Private tab password…”**. With a password set, your private file is **encrypted** before upload, so even someone who can open the repo on GitHub (like the other person sharing it) can’t read it — only someone with the password can. The password is remembered on this device and re‑entered on a new one; there’s no recovery if you forget it, so keep it safe. (Without a password, a private page is still hidden from other people’s app, but the file’s contents would be readable by anyone who browses the repo directly — set a password if that matters.)

### Storage (archive old tabs & labels — without deleting)
- **Put things away, don’t lose them:** right‑click a tab → **“Move to storage 🗄️”**, or right‑click a label → **“Move to storage 🗄️”** (you can also send a whole multi‑selection of labels at once). The item disappears from the tab bar / sheet but is fully kept.
- **The storage symbol:** a small **🗄️ archive button** sits to the right of the tabs, with a count badge when something’s inside. Click it to open storage.
- **Restore or delete:** the storage panel lists your stored **Tabs** and **Labels** (each label shows which tab it came from). **Restore** puts it back — a label returns to its original tab — or **Delete** removes it for good (that one asks you to confirm).
- **Nothing is really gone:** stored items are still saved and **synced/backed up** exactly like normal — and **private ones stay private** (kept in your own area, hidden from the other person). They just don’t clutter your tabs, and they’re kept out of Search until you restore them.
- One tab always stays out of storage, so your notebook is never empty.

### Search (find which tab or page has your words)
- **Where:** the **“Search”** button at the top‑right, or **⌘F / Ctrl‑F** from anywhere (it replaces the browser’s own find, which would only see the page you’re currently looking at).
- **What it covers:** every tab name, every label (its name *and* its page text), and every writing page — across the whole notebook at once, including your private tabs. Each result tells you **which tab** and **which label or page** the words are in.
- **Words or phrases:** type one word, or several to require **all** of them (e.g. `budget offsite` finds pages that contain both). Put **"quotes"** around text to match that **exact phrase** (e.g. `"next quarter"`).
- **Grouped by tab:** results are clustered under each tab’s name, with a count, so you can see at a glance which tabs contain your words (the top line says e.g. “4 matches in 3 tabs”). Click a tab heading to jump straight to that tab.
- **Sort the results:** a small **Sort** control in the search bar reorders them — **Best match** (default), **Recently edited**, **Tab name (A–Z)**, or **Name (A–Z)**. Your choice is remembered.
- **Jump to it:** click a result — or use **↑ / ↓** and **Enter** — to open that page, with the **first match highlighted** so you can see it right away. Each result shows a short preview with your words highlighted.

### Writing (the editor)
- **Fonts:** 10 choices (Arial is the default) — Menu also lets you set the label font separately.
- **Size** and **line spacing** (Single … Double) — line spacing applies to the paragraphs you select.
- **Page view** (the Continuous / Pages dropdown): keep a page as one long **Continuous** sheet, or **split it into separate page cards** (Letter or A4) that look and print like Microsoft Word’s Print Layout. Each sheet remembers its own choice, and the last choice becomes the default for new sheets. Printing and Save‑as‑PDF produce real separate pages either way.
- **Page numbers**: optional, and chosen right next to the page‑view control in the toolbar. When a sheet is set to “Pages”, a second dropdown appears — **No page #**, **Page # · center**, or **Page # · right**. It’s remembered per sheet, and your last choice becomes the default for new sheets. Page numbers are baked into **PDF** and **Word** exports too (Word gets a live, auto‑updating page number).
- **Print** (the printer button in the toolbar, or **⌘/Ctrl‑P**): opens your computer’s print dialog, which lists all of your installed printers (and “Save as PDF”) — just pick one. What prints matches the page view you chose: “Pages” sheets print as real Letter/A4 pages with your page numbers. You can also print a label’s page straight from the sheet by right‑clicking it → **Save or print → Print / PDF…**.
- **Bold, Italic, Underline, Strikethrough.**
- **Text color** (24) and **Highlight** (8 colors + “no highlight”).
- **Eyedropper — copy formatting** (the 🎯 button in the toolbar): click it, then click any text on the page, and IdeaSink copies **that text’s whole look — size, color, font, *and* style (bold, italic, underline, strikethrough)**. If you had text selected, it’s applied to your selection right away; if not, the formatting loads in so the next thing you type matches. Great for making one bit of text look exactly like another without redoing each button. Press **Esc** to cancel.
- **Pick a color from the screen** (in the text‑color and highlight menus, “🎯 Pick from screen…”): grabs the exact color of *any pixel on your screen* — a photo, an imported PDF page, anything — and uses it as your text or highlight color. Chrome/Edge only (it uses the browser’s built‑in screen color picker).
- **Bulleted and numbered lists** — Tab / Shift‑Tab to indent, Enter on an empty bullet to leave the list.
- **Hyperlinks:** select text → right‑click → Add hyperlink (⌘/Ctrl‑click a link to open it).
- **Undo / Redo:** the ↶ ↷ buttons, or ⌘Z / ⌘⇧Z — **as many steps back as you like**. IdeaSink keeps its own history rather than relying on the browser's, so the steps are the size you'd expect: roughly **one word (or one action) per press**, not one letter. Each formatting change, paste, image, or table edit is its own step, and **Redo** walks the whole way forward again. The buttons dim when there's nothing left to undo or redo. Each label keeps its own history for the session.
- **Icon names on hover:** move the pointer near any toolbar icon and a small label appears right away — the tool's name plus its shortcut (e.g. **Bold ⌘B**). No need to land on the button exactly, and no waiting for the browser's slow tooltip.
- **Paste matches your page:** pasted text takes on the page’s font instead of the copied font (bold, italic, lists, and links are kept).
- **Text auto-fill** (Menu → **“Text auto-fill…”**): two optional writing helpers.
  - **Word suggestions as you type** — ***off* unless you turn it on** (the pop‑up list annoyed more than it helped, so it’s opt‑in as of v47). When enabled: after a couple of letters, a small list appears with likely words — drawn from what you’ve already written plus common English words. **Tab**/**Enter** accepts, ↑/↓ picks, typing on ignores.
  - **Your own shortcuts** (on by default; they only act on codes *you* define): e.g. `sig` → your sign‑off. Type the code then **space** (or **Tab**) and it becomes the full text; shortcuts can be multi‑line. Add, edit, or delete them in the same dialog. Everything you set is kept on this device.

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
- **Double‑click** an image for a full‑size zoom view — scrollable **edge to edge**, even when the image is far bigger than the window; right‑click for width presets, “View full size”, and **Image info** (shows exactly how many pixels a copy contains).

### PDFs (sharp)
- **Drag a PDF file onto a page** and its pages are rendered as **high‑resolution, sharp** images — much crisper than copy‑pasting from a PDF viewer. For multi‑page PDFs you choose which pages to insert.

### Tables
- Insert an **n × n** table from a grid picker.
- **Drag cell borders** to resize columns and rows; **right‑click** inside a table to add/delete rows and columns; **Tab** moves between cells.

### Files on a page (attachments)
- **Any file — code, Word docs, spreadsheets, zips — can live on a label's page.** Drag it onto the page (or use the **📎 attach** button) and it becomes a small **chip** showing its name and size, sitting right in the text where you put it.
- **Stored inside the notebook**, so attachments ride along with **automatic backups and GitHub sync** — your wife's IdeaSink gets the files too, and they survive a browser wipe like everything else.
- **Click a chip** to save a copy to Downloads. **Right‑click** it for *View as text* (great for code — shows the file in a scrollable monospace view), *File info*, or *Remove*.
- **Search finds attachments by filename**, like everything else.
- Sizes: files up to **80 MB** each can be attached; anything over ~10 MB gets a heads‑up that it will slow that label's sync. Word/print exports show a small **name marker** in place of each file (the file itself can't ride inside a printout).

### Linked folder (a real folder on your computer, per page)
- The **📁 folder** button in the editor links a page to a **real folder on your disk** — a live view of its contents opens right in IdeaSink: each file with a **⬇** button (save a copy to Downloads) and a **📎** button (store a copy into the notebook as a chip).
- The link is **per‑computer** and IdeaSink itself never uploads or backs up the folder — it's a window onto your disk. That said, **if the folder you pick is a OneDrive/Dropbox folder, its files are of course already online** — kept there by that app, separately from IdeaSink's own protections (which cover your notes and 📎 attachments). The panel's wording reflects whichever case applies. (The other person sees only the folder's *name*; they can link their own copy on their machine, or ignore it.)
- Chrome and Edge only (Safari doesn't allow folder access), and the browser re‑asks permission after a restart — that's the browser being careful, not a bug.
- **Or paste a link instead.** If the folder is a **shared OneDrive folder** that's hard to find in the picker, choose **📁 → “Paste a link…”** and paste its share link. IdeaSink saves the link on the page — and since it's just a link, it **syncs to the other person too**, with an **Open online ↗** button for both of you. It then walks you through the one‑time OneDrive step (*open the link → “Add shortcut to My files”*) that makes the shared folder appear inside your local OneDrive folder, where you can pick it like any other. Dropbox and Google Drive links work the same way with their own “add/sync” options.
- Why the extra step? Browsers can't read OneDrive over the web without signing in (Microsoft requires it) — the OneDrive app on your computer is what bridges cloud and disk. Once the shortcut exists, IdeaSink reads the local synced copy, and OneDrive keeps it current.
- Rule of thumb: **attach** what should belong to the notebook and sync; **link** a folder you already keep on disk and just want at hand.

### Saving & backups

**Please read this one.** IdeaSink autosaves everything into your browser’s own storage. That is what makes it instant and offline — but browser storage is *temporary by design*, and the browser will throw it away without asking you first. Clearing browsing data, choosing “cookies and site data” in a cleanup, resetting the browser, or a tune‑up utility tidying website storage will erase every note in one go. There is no undo and no copy in the cloud. Nothing carries across to a different browser, a different computer, or a new profile either.

The fix takes about five seconds: pick a folder on your computer, and IdeaSink keeps a full copy there from then on, by itself.

- **Menu → “Automatic backup…” → “Choose backup folder…”** — pick your IdeaSink folder (or any folder). IdeaSink writes a single `IdeaSink-autobackup.json` there every few minutes, only when something has actually changed. An optional checkbox also keeps one dated copy per day, giving you a short history to fall back on.
- Until you have done that, IdeaSink says so: a yellow bar sits at the bottom of the window, and once a day it opens a short reminder explaining the risk. **Both disappear for good the moment a backup folder is set** — the bar is not a nag you have to live with, it is telling you your writing has nowhere safe to go. “Not now” hides the bar until you next open IdeaSink.
- **Menu → “Back up notes”** downloads a single JSON file of everything, any time you want a copy in hand; **“Restore backup”** loads one back in (it *merges*, keeping the newer version of each label). The automatic backup file works with Restore too — one file brings back the whole notebook.
- Safari and other browsers that can’t write straight into a folder get the download route instead: a backup file lands in **Downloads** on each interval, again only when something changed.
- Live sync (below) puts a copy in GitHub, which is real protection against losing this computer — but it is not a substitute for a local folder, and IdeaSink will still ask for one.

**Cloud folders (OneDrive, Dropbox, iCloud Drive) work — and are a good idea for backups.** A OneDrive folder looks like any normal folder to the browser; the OneDrive app quietly uploads whatever lands in it. So if you pick a OneDrive‑synced folder as the **backup folder** (or as a page’s **linked folder**), everything works as usual, and your backup additionally gets an off‑computer copy for free. Two things to know:

- **Turn off “online‑only” for that folder.** OneDrive’s *Free up space* / Files On‑Demand (and iCloud’s *Optimize Storage*) can turn files into cloud placeholders; right‑click the folder → **“Always keep on this device”** so the browser always finds real files.
- **The notebook itself doesn’t live in the folder.** Your *notes* live inside the browser on each computer — putting `IdeaSink.html` into OneDrive does **not** make the notebook follow you to another machine, and two people opening it from the same OneDrive do **not** share notes. On a new computer you’d open the file and use **Restore backup** (pointing at the autobackup JSON in that same cloud folder — convenient!), or turn on Live sync. For actually *sharing* with another person, GitHub Live sync remains the mechanism — a cloud drive can’t merge two people’s edits and would silently overwrite one of them.

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
- **By default: inside your browser on this computer**, and nowhere else. It is private and it is fast, but it is *not* safe storage — see the warning under “Saving & backups”. Clearing browsing data wipes it; each browser keeps its own separate copy.
- **With Automatic backup on:** also as `IdeaSink-autobackup.json` in the folder you chose, rewritten whenever something changes. This is the copy that survives a browser wipe, so set it up on day one.
- **With Live sync on:** also in your private GitHub repository, which additionally protects you if the computer itself is lost.
- Nothing is ever sent anywhere unless you turn Live sync on yourself.

## Good to know
- Use the **same browser** on a given computer, or your notes will look missing (each browser keeps its own copy). Sync or a restored backup brings them together.
- **Never “clear browsing data” without a backup folder set.** That single click is the one thing that can lose a whole notebook.
- Keep only one copy of `IdeaSink.html` in your folder to avoid opening an old version by mistake; the Menu shows the version number so you can confirm.

---

## License

*(Also shown inside the app: **Menu → “About & license”**.)*

Copyright © 2026 Larry Wu and Polly Hsu. All rights reserved.

Permission is granted to use, copy, and modify this software **free of charge for
personal, educational, and academic research purposes**, provided this notice and
the copyright line above are kept with any copy you pass on.

**Redistribution, commercial use, or inclusion in a commercial product or service
requires written permission from the copyright holders.**

The software is provided “as is”, without warranty of any kind, express or
implied. The authors are not liable for any claim, damages, or data loss arising
from its use. (Keep backups — see “Saving & backups” above.)

### Third-party software
IdeaSink embeds **Mozilla pdf.js 6.1.200**, used under the **Apache License 2.0**
— © Mozilla Foundation. It is what renders imported PDF pages. Its full licence
notice travels inside `IdeaSink.html` itself, so the requirement is satisfied by
the file as shipped; the licence text is at
<http://www.apache.org/licenses/LICENSE-2.0>. Nothing else third-party is
included — no fonts, no CDNs, no analytics.

*IdeaSink v50*
