# Hanzi Grader PWA

Public app shell for the Hanzi Grader. The mnemonic database and GitHub access token are **not** committed here.

## Complete setup

1. Upload the current small grader HTML file as **grader.html** in this repository's root. Do not upload the JSON database or token.
2. In GitHub Settings → Pages, set **Deploy from a branch**, branch **main**, folder **/(root)**, then Save.
3. Visit https://someone7070.github.io/hanzi-grader/ and import your private Hanzi_Data_v010.json through the grader's file picker. Browser storage is scoped to this new URL; prior local-file edits will not migrate automatically. Export/import a backup if necessary.
4. In Android Chrome, use ⋮ → Add to Home screen → Install.

The service worker caches the public app shell and fetched grader HTML. The private JSON database is cached by the grader in IndexedDB after import. Browser storage can be cleared; keep backups. The installed app requires an initial online visit and import before offline use.

## Privacy

Do not commit the private mnemonic database, personal access tokens, or incoming/approved private patches to this public repository. The app uses a separate private repository for authenticated patch synchronization.
