# PhD Council Event Invite Guide

A single-page, step-by-step guide that walks a first-timer through setting up a
**Microsoft Power Automate** flow: when someone registers for an event via
**Microsoft Forms**, they automatically get a confirmation email with a calendar
(`.ics`) invite attached.

Built for the **UHasselt PhD Council**, but the steps work for any event.

🔗 **Live page:** `https://vipul-chalo.github.io/phd-council-event-flow/`
*(fill in once GitHub Pages is enabled — see below)*

---

## What's in this repo

| File | What it is |
|------|------------|
| `index.html` | The entire guide — one self-contained HTML file. No build step, no dependencies to install. |
| `README.md` | This file. |

The page pulls two fonts from Google Fonts at load time; if those ever fail to
load, it falls back to a system font and still works.

---

## Publish it with GitHub Pages

1. Push this repo to GitHub (keep it **public** — GitHub Pages is free for public repos).
2. In the repo, go to **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder, then **Save**.
5. Wait ~1 minute. Your page goes live at
   `https://<your-username>.github.io/<repo-name>/`.

Because `index.html` sits at the repo root, GitHub serves it automatically — no
configuration needed.

---

## Updating the guide

Edit `index.html` and commit the change. GitHub Pages redeploys within a minute or two.

- **Text and steps** live in the `<body>` as plain HTML — search for the step title
  you want to change.
- **Colours and styling** are CSS variables near the top of the file (the `:root { … }`
  block) — change a hex value there to restyle the whole page.
- The page saves each reader's *"Mark done"* progress in their own browser
  (`localStorage`) only. Nothing is collected or sent anywhere.

After editing, open the file locally (double-click it) to check it before pushing.

---

## Good to know

- **No backend, no tracking, no cost.** It's a static page — nothing runs on a server.
- **Hosted on a personal account.** This repo lives under an individual GitHub account.
  If that person leaves the council, transfer the repo (or the whole account's ownership
  of it) to whoever takes over, so the guide can still be updated. GitHub's
  **Settings → General → Transfer ownership** moves a repo to another account or org
  without losing the URL history.
- **The `.ics` timezone** is set to `Europe/Brussels` inside the guide's calendar
  template, so event times are correct year-round without manual UTC conversion.

---

## License

Internal guide for the UHasselt PhD Council. Reuse and adapt freely within the council.
