# Shape Wars V87.51 — easy GitHub website upload

This GitHub Pages edition is designed for the **GitHub website's Add file → Upload files** button. There are only **10 files**, instead of 798.

## Upload in one batch

1. **Extract** the ZIP on your computer. Do not upload the ZIP itself to GitHub Pages.
2. Open the extracted `Shape_Wars_V87_51_GitHub_Easy_Upload` folder.
3. Create a new GitHub repository at https://github.com/new (for example `shape-wars`).
4. On your repository's **Code** page, click **Add file → Upload files**. In the file picker, select **all files inside the extracted folder** (not the containing folder). You can use Ctrl+A / Command+A. All files belong in the repository root.
5. Choose **Commit changes**. GitHub allows up to 100 files per batch, so these **10 files** fit in a single batch. Each file is under 25 MB, including artwork packs.
6. Go to **Settings → Pages → Build and deployment → Deploy from a branch**; select `main`, `/(root)`, and **Save**.
7. Your published URL is `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.

## File structure

- `index.html` — playable game, loads asset bundles automatically.
- `asset-pack-01.js` through `asset-pack-07.js` — all 794 original media assets bundled as data URLs. **Do not rename or omit these.**
- `README.md` — this guide.
- `package-info.json` — packaging information.

No `assets` folder is required, and no GitHub Desktop, Git, or command line is needed for upload.

## Notes

- The game is fully static, with no server component. Campaign saves are local to each user's browser and GitHub Pages origin.
- Game code and artwork become publicly accessible when hosted in a public repository; only publish media that you have rights to share.
- These packs contain the original game media, rearranged without re-encoding the images or audio.
- The upload limit is per file: every file in this package is below GitHub's 25 MiB browser-upload threshold.
- For offline testing, a local web server (e.g. `python3 -m http.server 8000`) mirrors GitHub Pages more reliably than `file://`.
