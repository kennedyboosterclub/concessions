# Kennedy Concessions v13 – Larger TV Descriptions

This patch increases product-description text size while preserving the three-line limit and current 16:9 layout.

Editor guidance:
- Green: 0–150 characters (recommended)
- Yellow: 151–180 characters
- Red: 181–210 characters
- Maximum: 210 characters

Descriptions continue to display for Hot Food, Drinks, Snacks, Candy, Breakfast, and Meal Deals.

This patch intentionally does NOT include `menu-data.js` or the `assets` folder, so uploading these files will not overwrite the live menu data or product images already in GitHub.


## v14 layout update
Candy now uses the large right-side menu panel for longer candy descriptions. Breakfast has moved to the smaller lower center panel beneath Snacks. All editor, image, stock, description, and GitHub publishing features remain unchanged.


## v15 item reordering
Every editable section now includes Move Up and Move Down buttons. Reordering changes the array order in menu-data.js, so the TV display follows the exact editor order after publishing. This applies to Hot Food, Drinks, Snacks, Candy, Breakfast, and Meal Deals.


## v16 Candy row update
Candy now renders like the other product categories: each item has its own image, item name, up to three lines of description, and price. The old decorative category image under the Candy heading has been removed.

## v17 fixes
- Fixed Candy rows failing to render because of an undefined image helper.
- Restored Meal Deals rendering after Candy.
- Standardized all product price badges to the same gold/black style used by Hot Food.
