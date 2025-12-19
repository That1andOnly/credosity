 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index 4a09b98e26b65226299f5b6bcb8e28e6e1844ad6..4545ca6d568d1ab7afec81c0e157eb1a5cdfb6e0 100644
--- a/README.md
+++ b/README.md
@@ -1,2 +1,20 @@
-# credosity
-Direct, truthful credit guidance after financial chaos.
+# Credosity
+
+Direct, truthful credit guidance after financial chaos. Static HTML site, no build step.
+
+## Pages
+- `Index.html` — homepage: positioning, core promise, and quick navigation.
+- `Start-here.html` — calm map with first steps and lane-specific guidance.
+- `denied-next-3-moves.html` — focused next moves after a credit denial.
+- `about.html` — why Credosity exists, who it’s for, and the no-fake-promises standard.
+- `assets.html` — checklists, logs, and copy/paste scripts (download links coming soon).
+- `affiliate-disclosure.html` — how the site makes money and the hard line on honesty.
+- `privacy.html` — plain-language privacy policy.
+
+## Running locally
+Open any page directly in a browser, or serve the folder with a simple HTTP server:
+
+```bash
+python -m http.server 8000
+# then visit http://localhost:8000/Index.html
+```
 
EOF
)
