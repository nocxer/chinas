 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index cd24842892a8c573e3b481471a4b579081f39013..243839468f8acb0500b21efab2f1b465283ac980 100644
--- a/README.md
+++ b/README.md
@@ -1,2 +1,37 @@
-# chinas
-Ini Newe Tine Basa "You and I have work to Do"
+# Cinox Holdings Global Group Website
+
+A modern, responsive single-page corporate website for **Cinox Holdings Global Group**.
+
+## Run locally
+
+Open `index.html` directly in your browser, or serve this folder with a static web server:
+
+```bash
+python3 -m http.server 8000
+```
+
+Then visit `http://localhost:8000`.
+
+## Assets
+
+- `assets/cinox-logo.svg`: Cinox Holdings Global Group wordmark used in the header and hero.
+
+## GitHub Pages deployment
+
+This repo is configured to deploy automatically with GitHub Actions when changes are pushed to `main` or `master`.
+
+After the first successful workflow run, your site URL will be:
+
+`https://<your-github-username>.github.io/<repository-name>/`
+
+To enable it in GitHub:
+1. Go to **Settings → Pages**.
+2. Set **Source** to **GitHub Actions**.
+3. Push to `main` or run the workflow manually from **Actions**.
+
+
+## Downloadable package
+
+A ready-to-share archive is available at:
+
+- `dist/cinox-holdings-site.zip`
 
EOF
)
