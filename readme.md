## IMDb Distractless Image Scroll

Stops the sponsored interstitial from interrupting the IMDb photo gallery, so Next/Previous always move to the next photo.

### Scope

The extension only ever acts on `imdb.com` and its sub-domains. It requests host permissions for `*://*.imdb.com/*` only, and uses `declarativeNetRequestWithHostAccess` so Firefox will not apply its blocking rule anywhere else. It has no content scripts, no background script, and collects no data.

### Publishing New Version

1) Make changes to the source code.

2) Increment app's version in `manifest.json`.

3) Install `web-ext` with:

```shell
npm install -g web-ext
```

4) Run the following command in the project's root directory:

```shell
web-ext build
```

5) The *.zip archive with updated version will appear in `web-ext-artifacts` folder.

6) Upload the updated verion to and follow the instructions on https://addons.mozilla.org.