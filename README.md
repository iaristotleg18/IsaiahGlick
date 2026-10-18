# Isaiah Glick — personal site

A static site (HTML, CSS, JavaScript). No build step. Works on GitHub Pages as-is.

## Hidden features (shortcuts and hover)
Pressing P, R, L, I or M opens Portfolio, Resume, LinkedIn, Instagram or Maroon. Esc closes the resume. The letters are shown in each tile's corner.

Hover your cursor near the big name: the letters lift and turn blue as it passes. It is off on touch screens and for visitors with reduced motion.

The page also shows a small "Key: P R L I M to open a tile" line in the bottom right corner so visitors find the shortcuts.

## Publish on GitHub Pages
1. On github.com, click **New repository**. Name it `isaiahglick.github.io` (replace with your username) for a clean URL, or any name. Set it to **Public**.
2. Click **uploading an existing file**, drag in everything from this folder (`index.html`, `css`, `js`, `assets`), and commit.
3. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then Save.
4. After a minute your site is live at the URL shown on that page.

## Protect the portfolio (Google Drive)
The Portfolio tile links to your Drive folder. Google controls who can open it:
1. In Drive, right-click the folder → **Share**.
2. Under **General access**, set **Restricted**.
3. Add the email addresses of people you approve. They sign in with that Google account to view.
4. Anyone else who clicks sees Google's "Request access" screen, and the site's **Request access** button emails you.

Do not set the folder to "Anyone with the link", or the link in this site will open it for everyone.

## Contact layout
By default the email sits top left and the phone top right, on the same line. To stack both on the left instead, change `<html lang="en">` in `index.html` to `<html lang="en" data-contact="stacked">`.

## Icon and link preview
`favicon.svg`, `favicon.ico`, `favicon-32.png` and `apple-touch-icon.png` are the browser tab and home-screen icons. `assets/og-image.png` is the preview image shown when the link is shared. Many apps (iMessage, LinkedIn, Slack) need the full web address, so once your site is live, change `content="assets/og-image.png"` in `index.html` to the full URL, for example `https://yourname.github.io/assets/og-image.png`.

## Things you can edit
- `js/config.js`: email, phone, Chicago Maroon page, LinkedIn, Instagram handle, Drive folder link, resume file name.
- `assets/Isaiah-Glick-Resume.pdf`: replace with a new resume any time (keep the file name).
- `index.html`: the intro text and the five tiles (`<nav class="tiles">`). The Resume tile opens a formatted resume page (the `#v-resume` section in `index.html`) with a Download PDF button that serves the PDF in `assets/`. Edit both when your resume changes.
- `css/style.css`: colors are the variables at the top (`--bg` charcoal, `--blue` accent).

## Privacy note
The resume PDF in `assets/` is public once the site is live, and it includes a phone number. Remove the phone number from the PDF if you don't want it public.
