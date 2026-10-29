ScanNet Scan-to-BEM Results - static website (no server code needed)

Contents: index.html + data/ (scenes.json, 312 point files, thumbnails). Keep the folder structure as it is.

Host it (pick one), then embed the public URL in Google Sites: Insert > Embed > By URL (choose "Whole page"),
and drag the embed box to about 1600 px tall.

  GitHub Pages:  new public repository -> upload the CONTENTS of this folder (index.html at the top level)
                 -> Settings > Pages > Deploy from branch "main", folder "/ (root)".
                 Web upload takes 100 files at a time, so use GitHub Desktop or:
                   git init; git add .; git commit -m site; git branch -M main
                   git remote add origin https://github.com/<you>/<repo>.git; git push -u origin main
                 URL: https://<you>.github.io/<repo>/
  Netlify Drop:  drag this folder onto https://app.netlify.com/drop
  FBK web space: copy the folder to any web server directory.

Test locally:  python -m http.server 8000  (inside this folder) -> http://localhost:8000
Opening index.html by double-click will not load the data (browsers block file:// fetches).
Deep link to one scan: https://.../index.html#scene0025_00
