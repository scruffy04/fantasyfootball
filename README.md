# Fantasy Draft Board PWA

This package is ready for GitHub Pages and works from a project repository URL such as:

`https://USERNAME.github.io/REPOSITORY/`

## Files to place in the repository root

- `index.html`
- `manifest.webmanifest`
- `service-worker.js`
- `icons/`

Commit and push those files to the branch used by GitHub Pages.

## GitHub Pages

In GitHub:

1. Open the repository.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Choose your branch (usually `main`) and `/ (root)`.
5. Save.

After GitHub publishes the site, open the GitHub Pages URL in Safari on iPhone/iPad.

## Add to iPhone or iPad

1. Open the site in **Safari**.
2. Tap **Share**.
3. Choose **Add to Home Screen**.
4. Tap **Add**.

It will launch in standalone app mode with its own icon.

## Updating the draft board

Replace `index.html` with the newest board version, but keep the PWA metadata and service-worker registration in the file.

If you substantially change the app and an iPhone/iPad keeps showing an old cached version, increment `CACHE_NAME` in `service-worker.js`, e.g. from `v1` to `v2`, commit, and refresh the site once in Safari.
