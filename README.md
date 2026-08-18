# Kennedy Football Concessions – v7 editor fix

Upload all files/folders in this package to the existing `kennedyboosterclub/concessions` repository and replace the existing versions.

## What v7 fixes
- Restores all five editable product groups: Hot Food, Drinks, Snacks, Candy, and Meal Deals.
- Adds the missing **Test GitHub Connection** button.
- Initializes the product editor before GitHub publishing controls, so a publishing-script issue cannot make the product sections disappear.
- Keeps product photo upload, QR upload, descriptions, prices, add/remove item controls, preview, backup/restore, and direct publishing.
- GitHub publishing fetches the current `menu-data.js` SHA before every update and retries one SHA conflict automatically.

## After upload
GitHub Pages/browser caching may briefly show the older editor. After the commit finishes, open:

`https://kennedyboosterclub.github.io/concessions/editor.html?v=7`

The `?v=7` is only a cache-buster. You can later use the normal editor URL.

Before publishing, click **Test GitHub Connection**. A successful test confirms that the browser can read `menu-data.js` with the token. The token needs repository `Contents: Read and write` access.
