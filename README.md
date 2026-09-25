# Bag Charm Studio

An English reading-and-design game with 10 customers, 9 backpack colours and 40 decorations. Each customer needs one bag and four pieces that match her story. All 40 pieces are used across the 10 rounds.

## Play
Open `index.html` in a modern browser. No build, account, internet connection or external dependencies are required.

1. Read the customer's story at the bottom.
2. Choose a backpack from the right-hand list.
3. Select a piece from the two-column collection, then select an attachment spot. Desktop users can also drag pieces onto spots.
4. The game checks automatically. A new selection replaces an attached piece; activating a piece without a selection removes it. Each piece can appear once per bag.
5. Match the colour and all four pieces to unlock the next customer. After round 10, view the completed collection.

Use the search field to find a piece. Buttons support keyboard navigation with Tab and Enter or Space. Progress is saved on this browser when local storage is available. Browser privacy settings or file URL restrictions may prevent saving; gameplay still works.

## GitHub Pages
Extract the ZIP. Upload the **contents** of `bag-charm-studio` to your repository so `index.html`, `style.css`, `data.js`, `app.js` and the `assets` folder are at the repository root. Do not upload only the ZIP.

In the repository's Settings → Pages, choose deployment from a branch, select your branch and the root folder, and save. Use the published Pages link after deployment completes.

## Files and assets
All imagery was supplied for this project. The 60 images are packaged as high-quality WebP files to reduce download size; RGB compression is lossy. Original source images are untouched. All asset paths are relative, so the game also works in a repository subdirectory. There are no tracking scripts, remote fonts or network requests to external services.

Nine full-size backpacks were supplied. Pink is used for two distinct customer stories. The miniature decorated backpack is a charm, not a selectable full-size bag.

Edit `ROUNDS` in `data.js` to change stories and answers. `assess()` checks the colour, exactly four distinct pieces, and the required set independently of placement order. The interface is intentionally non-punitive: players may revise choices until they match.

## Simple English edition

Stories use short first-person sentences, present simple, colours, hobbies and days of the week. Clues describe familiar actions rather than listing the exact charm names. Some unusual items (such as axolotl and slime) are named to avoid unclear answers. This is not an official Spotlight curriculum alignment.

After the fourth piece is added, each attached piece shows a green tick for a correct choice or a red cross for an incorrect choice. The chosen bag also shows its colour result. Feedback stays visible while the player replaces or removes pieces and updates immediately. A new round clears the feedback.
