# Kennedy Football Concessions Digital Menu

## Files
- `index.html` — 16:9 TV menu for Fire TV / Silk Browser
- `editor.html` — menu editor with product image upload and direct GitHub publishing
- `menu-data.js` — menu content read by the TV page
- `assets/` — starter product and Kennedy artwork

## Editor workflow
1. Open `https://kennedyboosterclub.github.io/concessions/editor.html`.
2. Edit products, prices, descriptions, headings, payment information, or meal deals.
3. For any product, click **Choose Image** and select a photo from your phone/computer. The editor automatically resizes and compresses it and embeds it into `menu-data.js`, so no separate image upload is required.
4. Click **Refresh Preview** to see the TV board.
5. Enter a GitHub fine-grained personal access token with repository access limited to `kennedyboosterclub/concessions` and permission **Contents: Read and write**.
6. Click **SAVE & PUBLISH TO TV**. The editor updates `menu-data.js` through GitHub's API. GitHub Pages then rebuilds automatically.
7. Refresh the Fire TV menu after the deployment completes.

## Token safety
The editor does not place your token in the repository or menu data. It stores the token only in `sessionStorage`, which lasts for the current browser session. Use a fine-grained token restricted to this one repository and only the permissions required for updating repository contents.

## Manual fallback
The editor can still download `menu-data.js`. If direct publishing is ever unavailable, upload that one file to the repository root and commit it manually.
