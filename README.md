# Craftique — Standalone Website

This is your complete website as a single file: `index.html`.
No build tools, no installs — just upload it.

## Why this fixes your phone problem

The link you were using before was a Claude "artifact" link. Those only work
properly inside Claude's own app/website — that's why your phone kept trying
to open the Claude app, and why product photos got stuck on "Loading…"
(they were waiting on a Claude-only connection that doesn't exist outside
Claude's app).

This file does **not** depend on Claude at all. Once it's hosted on a normal
website address, it will:
- Open directly, instantly, on any phone or computer — no app prompts
- Show all 16 of your real product photos immediately (they're built
  directly into the file, not loaded from anywhere else)
- Work completely offline-capable for browsing once loaded

## The one tradeoff

Without Claude's app, there's no shared online database. So when you use
the **Admin panel** (password: `craftique2026`) to add/edit/delete products
or change settings, those changes save to **that browser only** — they
won't automatically appear for customers visiting from their own phones.

For a personal/family-run shop, the simplest way to manage this:
1. Make all your edits once, from one browser, until you're happy with the site
2. Re-export/re-upload the updated file to your host whenever you make changes

(If you want everyone's edits to sync live for all visitors automatically,
that needs a real backend + database — a bigger project. Ask me anytime if
you want to go that route later.)

## How to publish this for free (pick one)

### Option A — Netlify Drop (easiest, 2 minutes, free)
1. Go to https://app.netlify.com/drop
2. Drag the `index.html` file straight onto the page
3. You instantly get a live URL like `https://random-name-123.netlify.app`
4. Share that link anywhere — it just works, on any phone

### Option B — GitHub Pages (free, your own GitHub username in the URL)
1. Create a free GitHub account if you don't have one: https://github.com/signup
2. Create a new repository, name it anything (e.g. `craftique`)
3. Upload `index.html` into it (use "Add file" → "Upload files" in the repo)
4. Go to repo Settings → Pages → set source to "main" branch, root folder
5. Your site will be live at `https://yourusername.github.io/craftique/`

### Option C — Your own domain (paid hosting, e.g. Hostinger/GoDaddy)
1. Log into your hosting control panel (often called cPanel or File Manager)
2. Find the folder usually called `public_html` or `www`
3. Upload `index.html` into that folder
4. Visit your domain — it will load this site automatically

## Changing the admin password

Open `index.html` in any text editor, search for:
```
const DEFAULT_PASSWORD = "craftique2026";
```
Change the text between the quotes to whatever you like, save, and
re-upload the file to your host.

## Adding/editing products after hosting

Open your live site in a browser → scroll to the very bottom → tap
**"Admin login"** → log in → use the Products tab to add, edit, or delete
items, the Site Content tab to change text, and Account & Security to
change your password or Instagram handle.

Remember: these edits save to that one browser only (see "the one
tradeoff" above).
