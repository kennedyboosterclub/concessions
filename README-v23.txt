Kennedy Concessions v23 — Large Draft Storage Fix

SAFE UPDATE:
Replace editor.html only.
Do not replace index.html or menu-data.js.

What changed:
- Local editor drafts now use IndexedDB instead of localStorage.
- IndexedDB can hold substantially more data, which is important because product and sponsor images are embedded in the menu.
- Sponsors, logos, ordering, active/hidden state, prices, descriptions, products, and other editor changes survive refreshes.
- The small localStorage preview cache is now optional; if it fills up, it no longer causes an editor-save error.
- Publishing to GitHub is unchanged.
- Reset clears the IndexedDB draft and reloads the menu version provided by GitHub Pages.
