Kennedy Concessions v22 — Editor Sponsor Persistence Fix

SAFE UPDATE:
Upload editor.html over the existing editor.html in GitHub.
You do not need to replace index.html or menu-data.js.

Fix:
- The editor now automatically saves the complete working menu to browser storage.
- Sponsors, sponsor logos, rotation order, active/hidden state, and rotation time survive an editor-page refresh.
- Other editor changes also receive the same local-draft protection.
- Publishing to GitHub still works exactly as before.
- After a successful publish, the local draft is retained so a temporarily cached GitHub Pages copy cannot make newly added sponsors disappear.
- Reset still returns the editor to the published menu version loaded by the page.

Note:
Browser localStorage has a size limit. Because product/sponsor images are embedded as compressed data, extremely large numbers of images can eventually fill browser storage. The editor will show an error if that happens.
