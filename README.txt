# हिसाब-किताब · Split Ledger — Installable PWA

Files:
- index.html — your app with PWA metadata and service-worker registration
- manifest.json — install/app metadata
- sw.js — app-shell service worker
- icon-192.png — Android/web icon
- icon-512.png — large install icon

IMPORTANT:
1. Deploy these files from a web host that supports HTTPS.
2. Keep all files in the same folder.
3. Do NOT open index.html directly with file:// if you want installation.
4. Your existing Google Apps Script API remains the backend; the service worker deliberately does not cache its requests.

For Google Apps Script:
- A Google Apps Script web app itself is not a normal static-file host for a multi-file PWA.
- Host these PWA files on a free HTTPS static host (for example GitHub Pages or Cloudflare Pages), while leaving your existing API URL in index.html unchanged.

On Android Chrome:
- Open the HTTPS app URL.
- Use the browser menu and choose "Install app" / "Add to Home screen" (wording can vary).
- The generated icon will be used.

On desktop Chrome/Edge:
- Open the HTTPS app URL.
- Use the install icon in the address bar or browser menu.
