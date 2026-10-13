JuniorFirst — Student Study Library
===================================
Free notes, previous year papers (PYQ) and syllabus for every department at
Bundelkhand University, Jhansi. No senior, no paywall, no ragging.

Built and owned by Gaurav Kumar. (c) 2026. Please do not copy or re-host this
site or its code without permission.

This folder is a complete, ready-to-host website AND an installable app (PWA).
One codebase gives you both a website and a phone app — no Play Store needed.


WHAT'S IN THIS FOLDER
---------------------
index.html            The whole website (all design + logic in one file)
manifest.webmanifest  Tells phones the site can be installed as an app
sw.js                 Service worker — makes it work offline after first visit
icons/                App icons (192, 512, apple-touch-icon)


DEPARTMENTS COVERED (10)
------------------------
First Year (Common) · Electrical · Mechanical · Civil · CSE · ECE ·
Electronics & Instrumentation · Biotechnology · Food Technology · Biomedical


PUT IT ONLINE (FREE) — pick ONE
-------------------------------
Option A — Netlify (easiest, ~2 minutes)
  1. Go to https://app.netlify.com/drop
  2. Drag this whole folder onto the page.
  3. You get a live link instantly. Rename it under Site settings.

Option B — GitHub Pages (good for a permanent free link)
  1. Create a new public repo, e.g. "juniorfirst".
  2. Upload every file from this folder (keep the icons/ folder).
  3. Settings -> Pages -> Source: "Deploy from a branch" -> main -> / (root).
  4. Your site goes live at  https://<your-username>.github.io/juniorfirst/

Note: install/offline features need https (both options above provide it).


TURN IT INTO AN APP (for students)
----------------------------------
Once hosted, a student opens the link on their phone:
  - Android (Chrome): an "Install app" button appears in the top bar, or
    menu -> "Add to Home screen".
  - iPhone (Safari): Share -> "Add to Home Screen".
The icon lands on their home screen, opens full-screen, and works offline.
That is the app — no separate download, no Play Store, no cost.


MAKE THE DOWNLOADS REAL
-----------------------
Right now every "Download PDF" button is a demo (href="#"). To go live:
  1. Put your PDFs in a Google Drive folder, share it "Anyone with the link".
  2. Open index.html in any text editor (Notepad is fine).
  3. Find  <a class="dl" href="#">  and replace the # with the Drive/PDF link.
  4. Repeat for each row. Save. Re-upload to your host.

Tip: use one Drive folder per department.


ADD A DEPARTMENT LATER
----------------------
In index.html find <select id="branchSelect"> and remove the word "disabled"
from an option, or add a new one. Then add subject cards with matching
data-branch="..." values (the filter chips and cards use the same value).


THIS PROJECT'S PURPOSE
----------------------
So no junior has to depend on a senior, pay for notes, or face pressure just
to get study material. Ragging is banned under UGC regulations in India.
Free access for everyone, always.


TURN ON DOWNLOADS & SUBMISSIONS (one place)
------------------------------------------
Open index.html in any text editor (Notepad is fine) and find these three
lines near the bottom, inside <script>:

  var DRIVE = '';      // paste your Google Drive folder link here
  var WHATSAPP = '';   // e.g. '919876543210'
  var EMAIL = '';      // e.g. 'you@example.com'

- DRIVE    -> every "Notes PDF" / "Formula sheet" / "Download PDF" button
              opens this folder in a new tab. Share the folder as
              "Anyone with the link".
- WHATSAPP -> the "Share your notes" form sends submissions straight to
              this number (country code, no + or spaces).
- EMAIL    -> set this instead if you prefer email submissions.

Save the file and re-upload. That is the only edit needed.


WHAT'S BUILT IN
---------------
- Tap any subject card -> a detail panel opens with Notes / PYQ / Formula
  sheet / Save buttons.
- A save (bookmark) icon on each card, plus a "Saved" filter that remembers
  choices on the device.
- A "Share your notes" form, opened from the banner, the footer or the
  Share tab.
- A mobile bottom tab bar (Branches, Subjects, PYQ, Share).
- Install-as-app (PWA), offline support and dark mode.
