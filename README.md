# Zumi

A personal running training calendar. Upload your Excel plan, see every run and gym session by week, log actual km and track planned vs actual in a weekly chart.

## Put it online with GitHub Pages (about 5 minutes)

1. Sign in at github.com and select **New repository**.
2. Name it `zumi`, set it to **Public**, and select **Create repository**.
3. On the empty repository page, select **uploading an existing file**.
4. Open this folder on your computer and drag **everything inside it** into the browser (index.html, manifest.json, sw.js, xlsx.full.min.js, README.md and the five .png icon files). Make sure `index.html` is at the top level, not inside a subfolder.
5. Select **Commit changes**.
6. Go to **Settings**, then **Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, choose branch **main** and folder **/ (root)**, then **Save**.
7. After a minute or two, the page shows your address: `https://YOUR-USERNAME.github.io/zumi/`

## Install it on your phone

- **iPhone (Safari):** open the address, tap Share, then **Add to Home Screen**.
- **Android (Chrome):** open the address, tap the menu (three dots), then **Install app** or **Add to Home screen**.

Open the app, choose **Choose Excel file** and upload your plan. Your plan and logged km are saved on that phone, and the app works offline after the first load.

## Notes

- Your data stays in your phone's browser storage. It is not uploaded anywhere. Clearing the browser's site data will erase it, so keep your Excel file.
- Upload the Excel file separately on each device you use.
- To update the app later, upload the changed files to the repository and, if the old version still shows, change `zumi-v2` in `sw.js` to `zumi-v2`.
- Excel reading uses SheetJS (Apache 2.0 licence), included as `xlsx.full.min.js`.

## If Android says it can't be installed

1. Open the address in **Chrome** (not Samsung Internet, Firefox or a link opened inside another app), and not in a private tab.
2. Check the address is your GitHub Pages one, ending in `github.io/zumi/`.
3. Visit `https://YOUR-USERNAME.github.io/zumi/manifest.json` and `.../sw.js`. Both should show text. If you see "404", the files were uploaded into a subfolder: `index.html` must sit at the top level of the repository.
4. Wait a minute, reload the page twice, then open Chrome's menu again. Look for **Install app**.
5. If it is already installed once, Chrome won't offer it again. Remove the old shortcut first.
