# START HERE — the GitHub **profile view**, end to end

The thing you land on at **github.com/Akr246**. Browser only, no terminal, about 15 minutes.

```
2-profile-repo/         →  repo: Akr246              ← START HERE, this is the profile view
   README.md
   profile-assets/      ← new folder: the dark panels
1-portfolio-repo/       →  repo: Akr246.github.io    (the website — already updated last round)
3-spendlens-repo/       →  repo: spendlens-ai-spend-intelligence
resumes-to-apply-with/  →  keep on your computer
preview/                →  what it will look like, light and dark theme
```

---

## First, the one thing GitHub won't let you do

**GitHub controls the profile page background.** There is no setting, anywhere, that changes it —
it is white in light theme and `#0d1117` in dark theme, and it follows *the visitor's* preference,
not yours. Anyone who tells you otherwise is selling something.

So the way you get a website look is to **bring your own background inside the page.** Your README
now renders five full-width dark panels — each one an image carrying its own midnight-blue
background, its own gradient border, and its own icons. The GitHub page around them stays
whatever colour the visitor set, and your panels sit on top of it looking deliberate in both.

Open `preview/profile-view-light-theme.png` and `preview/profile-view-dark-theme.png` — same
README, both GitHub themes. That's the effect.

---

## What's in the new profile view

| Panel | What it carries |
|---|---|
| 🖼️ **hero** | Your photo inside a blue-to-mauve ring, name in Playfair-style serif, tagline, location with a pin icon, and three pills — MBA · Actively interviewing · Product/Analysis/Programme |
| 📊 **stats** | Four tiles with icon headers: 3 years · 500+ stakeholders · 10+ teams · 20% efficiency gain |
| 🔍 **focus** | 23 focus-area chips — the ATS keywords, visible rather than hidden |
| ⭐ **work** | SpendLens as the headline card, plus the two case-study cards |
| 🎯 **principles** | The four things about how you work, each on its own coloured-edge row |

Around the panels, still as real searchable text: badge buttons for Portfolio · Case Studies ·
LinkedIn · Credly · Email · Live app, five role-tagged resume download badges, an icon-led
experience table, twenty technology badges, education and certifications side by side, and
GitHub stats cards themed to the same palette.

Every panel ships twice — `.svg` (what the README uses: crisp at any size, ~28 KB) and `.png`
(a fallback, in case an SVG ever refuses to render). You don't need to do anything with the PNGs.

---

## PART 1 · The profile view — repo `Akr246`

> This repo has the same name as your username. That's what makes it the profile view.
> If it doesn't exist yet: **New repository** → name it exactly `Akr246` → tick
> **Add a README file** → **Create repository**.

### Step 1 — upload the panels folder

1. Go to **github.com/Akr246/Akr246**
2. **Add file → Upload files**
3. Drag the whole **`profile-assets`** folder from `2-profile-repo` into the drop area
4. Commit message: `Add profile panels`
5. **Commit changes**

**Check before moving on:** the repo file list should now show a `profile-assets` folder, and
opening it should show **10 files** (5 `.svg` and 5 `.png`). If you see fewer, or no folder at
all, the drag didn't take — try again by dragging the files themselves rather than the folder,
then rename the path in the upload box to `profile-assets/`.

> This step has to be **first**. If you paste the README before the images exist, you'll get five
> broken-image icons and think it's broken. It isn't — it just can't find the pictures yet.

### Step 2 — paste the README

1. Still in `github.com/Akr246`, click **`README.md`**
2. Click the **pencil icon** (top right of the file)
3. Click inside the text, select all *(Ctrl+A / Cmd+A)*, delete
4. Open `2-profile-repo/README.md` in Notepad or TextEdit, select all, copy
5. Paste it into the GitHub editor
6. Commit message: `Iconified profile view with dark panels`
7. **Commit changes**

### Step 3 — look at it

Go to **github.com/Akr246**. You should see the hero panel first, then the badge row, then the
stat tiles.

**If a panel shows as a broken image:** give it 30 seconds and hard-refresh *(Ctrl+Shift+R)* —
GitHub caches images through its own proxy and the very first load can miss. If it's still broken
after that, the `profile-assets` folder didn't upload; redo Step 1.

**If you'd rather use the PNGs:** in the README, change every `./profile-assets/hero.svg` to
`./profile-assets/hero.png` — same for `stats`, `focus`, `work`, `principles`. Five edits.

---

## PART 2 · Website — repo `Akr246.github.io`

Unchanged from last round. If you haven't uploaded it yet:

1. **Add file → Upload files**
2. Drag in all five items from `1-portfolio-repo`: `index.html`, `case-studies.html`,
   `PROJECTS.md`, the `assets` folder, the `resumes` folder
3. **Commit changes**

> If the folders don't come across, upload the three files first and commit, then do a second
> upload with only `assets`, and a third with only `resumes`.

⚠️ **Before you publish this one:** `case-studies.html` still has three purple "Fill this in"
boxes at lines 132, 137 and 161 — the Align Technē automation specifics, one honest thing you'd
do differently, and the Annalect A/B test metric. Fill them or delete the `<div>` blocks.

---

## PART 3 · SpendLens — repo `spendlens-ai-spend-intelligence`

Open its `README.md` → **pencil icon** → select all, delete → paste `3-spendlens-repo/README.md`
→ **Commit changes**.

---

## PART 4 · The profile view settings GitHub *does* let you change

These are on the profile page itself, not in a repo — and they're what most people forget.

1. **Bio and links.** Click your avatar (top right) → **Your profile** → **Edit profile**.
   - **Bio:** `Product · Business analysis · Programme management. MBA AI for Business @ BITS Pilani. Building SpendLens.`
   - **Location:** `Bengaluru, India`
   - **Website:** `https://akr246.github.io`
   - **Social links:** LinkedIn `https://www.linkedin.com/in/akr246`, Credly `https://www.credly.com/users/arya-k-ravi`
   - Tick **Available for hire** — it puts a badge on your avatar and surfaces you in GitHub Jobs search.

2. **Pin your repos.** On the profile page, **Customize your pins** → pin
   `spendlens-ai-spend-intelligence` first, `Akr246.github.io` second. Pinned repos appear
   immediately under your README, so their descriptions are read as part of the profile.

3. **Repo descriptions.** On each repo, click the ⚙️ beside *About*:
   - `Akr246.github.io` → `Portfolio — product, analysis and programme work. Case studies and role-specific resumes.` · website `https://akr246.github.io`
   - `spendlens-ai-spend-intelligence` → `Behavioural spend-intelligence web app. React + TypeScript, six decision engines, fully client-side.` · website `https://akr246.github.io/spendlens-ai-spend-intelligence/`

4. **Topics.** On both repos, add: `product-management`, `business-analysis`,
   `product-analytics`, `react`, `typescript`, `portfolio`.

5. **Profile photo.** Use the same headshot as the hero panel, so the GitHub avatar and the
   panel match. Edit profile → click the avatar → upload `1-portfolio-repo/assets/arya.jpg`.

6. **Make your Credly profile public** — Credly → Settings → Privacy. Right now the Credly
   badge on your site and profile goes to a page a recruiter can't open.

---

## The order that avoids every problem

```
1.  Upload profile-assets/          →  repo Akr246
2.  Paste README.md                 →  repo Akr246
3.  Hard-refresh github.com/Akr246  →  confirm five panels render
4.  Edit profile: bio, links, available-for-hire
5.  Customize your pins
6.  Repo descriptions + topics
7.  Fill the three boxes in case-studies.html, then upload 1-portfolio-repo
8.  Paste the SpendLens README
9.  Make Credly public
```

---

## Still open — worth fixing

1. **Employer name.** The panels, site and resumes all say **Align Technē**. If the real spelling
   differs, tell me and I'll regenerate everything in one pass — the name is baked into the
   images, so this is not a find-and-replace you can do yourself.
2. **LinkedIn vs resume.** LinkedIn says *Annalect India* and MBA *April 2026*; the resumes say
   *Annalect India (Omnicom Group)* and *in progress*. Recruiters compare the two.
3. **The three `fill` boxes** in `case-studies.html`.

---

*The panels are generated images, so any wording change inside them needs a regenerate — ask and
you'll get a new `profile-assets` folder to drop in. Everything outside the panels is plain
markdown you can edit yourself in the GitHub editor.*
