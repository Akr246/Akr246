# START HERE — Arya K. Ravi · GitHub update kit

Everything you need, in the order you need it. Browser only, no terminal.
About 20 minutes start to finish.

```
1-portfolio-repo/        →  upload into  Akr246.github.io     (the portfolio website)
2-profile-repo/          →  upload into  Akr246               (your profile README)
resumes-to-apply-with/   →  keep on your computer            (attach to applications)
```

You are creating **two repositories**. A third — `spendlens-ai-spend-intelligence` — already
exists and needs nothing except the tidy-up in Part 5.

| Repo | Becomes | Lives at |
|---|---|---|
| `Akr246.github.io` | Portfolio website + all six resumes | akr246.github.io |
| `Akr246` | Profile README | github.com/Akr246 |

**Do Part 1 before Part 2.** The profile README links to the portfolio, so the portfolio
has to exist first.

---

# PART 1 · The portfolio website

### 1.1 Create the repository

Skip this if `Akr246.github.io` already exists.

1. Go to **https://github.com/new**
2. **Repository name:** `Akr246.github.io`
   Exactly your username, then `.github.io`. This exact name is what makes GitHub serve it
   as a website rather than just storing the files.
3. **Description** *(optional)*: `My portfolio — product, analysis and programme work. Live at akr246.github.io`
4. **Public**
5. Leave all three checkboxes **unticked**
6. **Create repository**

### 1.2 Upload the files

The folder structure matters. `assets/` and `resumes/` must arrive as folders, not loose files.

1. On the page that appears, click **uploading an existing file**
2. Open the `1-portfolio-repo` folder on your computer
3. Select **all three items** — `index.html`, the `assets` folder, and the `resumes` folder —
   and drag them into the browser together
4. Wait until the file list stops growing. There are 10 files; the video is ~1.4 MB and is
   the slow one. Give it 30 seconds.
5. Scroll to the bottom → **Commit changes**

**Verify before you continue.** The repo should now show `index.html` plus two folders.

> **If you only see `index.html`:** the folders did not come across. Do them separately —
> **Add file → Upload files**, drag only the `assets` folder, commit. Then repeat with
> `resumes`. This is the step that has failed before, so check it properly.

### 1.3 Turn on GitHub Pages

**Settings → Pages → Build and deployment**

- **Source:** Deploy from a branch
- **Branch:** `main`, folder `/ (root)`
- **Save**

Wait 1–2 minutes, then open **https://akr246.github.io**

**What you should see:** your photo inside a slowly rotating blue-to-mauve ring, the four
numbers counting up as you scroll, and five role tabs. Click a tab — the paragraph and the
resume download should both change.

> **404?** Wait another minute and hard-refresh with **Ctrl+Shift+R**. First deployments are
> often slow.

### 1.4 Add the About details

Back on the repo page, click the **gear icon** next to "About" on the right:

- **Website:** `https://akr246.github.io`
- Tick **"Use your GitHub Pages website"**
- **Topics:** `portfolio` `product-management` `business-analysis` `product-analytics`

---

# PART 2 · The profile README

### 2.1 Create the repository

Skip this if `Akr246` already exists.

1. **https://github.com/new**
2. **Repository name:** `Akr246` — exactly your username.
   GitHub displays a message with a sparkle emoji saying you found a secret. That is your
   confirmation you have it right.
3. **Description** *(optional)*: `My GitHub profile README`
4. **Public**
5. **Tick "Add a README file"** — this is the one and only time you want that box ticked
6. **Create repository**

### 2.2 Paste in the content

1. Click **README.md**
2. Click the **pencil icon** (Edit this file), top right
3. Select everything already there and delete it
4. Open `2-profile-repo/README.md` from the kit, copy the whole file, paste it in
5. **Commit changes…** → leave "Commit directly to the `main` branch" selected →
   **Commit changes**

Go to **https://github.com/Akr246**. The README now sits at the top of your profile.

**Verify:** click one of the five role-resume links. It should open the PDF from the
portfolio site you deployed in Part 1.

---

# PART 3 · Profile settings

On **github.com/Akr246**, click **Edit profile** (left column, under your photo).

**Bio** — your current one points recruiters at data-analyst roles, which is not what you
are applying for. Replace it with:

```
Psychology → product. I turn loose requirements into things teams can build. Ex-TPM @ Align Technē. MBA in AI for Business, in progress. Open to Product / BA / APM roles.
```

**Location:** `Bengaluru, India`

**Website:** `https://akr246.github.io`

**Company:** currently shows Codsoft — change to Alignerr, or clear it.

**Social accounts:** add your LinkedIn if it is not already there.

**Save.**

---

# PART 4 · Pinned repositories

Your profile currently pins **CODINGSAMURAI** and **testrepo**. A repository called
"testrepo" on a profile you are sending to employers reads as unfinished before anyone
clicks it.

On your profile → **Customize your pins**:

- **Tick** `spendlens-ai-spend-intelligence`
- **Untick** `testrepo`
- Keep `CODINGSAMURAI` only if the work inside is presentable — open it and check first
- **Save pins**

SpendLens should sit first in the order.

---

# PART 5 · Tidy the SpendLens repo

Open `spendlens-ai-spend-intelligence` → **gear icon** next to "About":

- **Description:** `Behavioural spend intelligence for Indian households — RED/GREEN priority classification, goal feasibility and pattern detection. React + TypeScript, runs entirely in the browser.`
- **Website:** `https://akr246.github.io/spendlens-ai-spend-intelligence/` and tick
  **"Use your GitHub Pages website"**
- **Topics:** `react` `typescript` `vite` `fintech` `personal-finance` `product-management` `data-visualization`

---

# Final checklist

- [ ] **akr246.github.io** loads — photo, rotating ring, counters animate
- [ ] Clicking a role tab swaps both the paragraph and the resume download
- [ ] The architecture video plays inside the SpendLens card
- [ ] **github.com/Akr246** shows the README at the top
- [ ] The five role-resume links in the README all open
- [ ] The **Credly** link works — *make sure that profile is set to public*
- [ ] Bio no longer says "Data Analyst"
- [ ] `testrepo` is unpinned; SpendLens is pinned first
- [ ] Open **akr246.github.io on your phone** — this is how most recruiters see it first

---

# Which resume goes where

| Applying for | Send this file |
|---|---|
| Product Associate | `Arya-K-Ravi-Product-Associate.pdf` |
| Associate Product Manager | `Arya-K-Ravi-Associate-Product-Manager.pdf` |
| Product Analyst | `Arya-K-Ravi-Product-Analyst.pdf` |
| Business Analyst | `Arya-K-Ravi-Business-Analyst.pdf` |
| Associate Program Manager | `Arya-K-Ravi-Associate-Program-Manager.pdf` |
| Unsure, or a mixed posting | `Arya-K-Ravi-Resume-General.pdf` |

All of them carry **identical facts**. What changes is which role is named at the top, which
competency group leads, and the order of bullets inside each job. The Product Analyst version
opens Annalect with the Tableau and A/B testing work; the Business Analyst version opens
Align Technē with the SAP migration. Nothing is added, removed or invented between versions.

The `.docx` files are included so you can edit them yourself later.

---

# Updating anything, later

**A resume** — upload the new PDF into the `resumes` folder of `Akr246.github.io` using the
**same filename**. It overwrites the old file and every link — portfolio, profile README,
anything you have already sent — keeps working. Never rename the files.

**Portfolio wording** — open `index.html` in the repo, pencil icon, edit, commit. Live in
about a minute. It is plain HTML; the text is readable and safe to change.

**Add a project card** — in `index.html`, find a block that starts
`<div class="card" style="margin-top:22px">`. Copy the entire block, paste it below itself,
and change the heading and paragraph.

**Change a role pitch** — near the bottom of `index.html`, find `const ROLES=[`. Each entry
has `k` (the tab label), `f` (the PDF filename) and `p` (the paragraph). Edit the text
between the quote marks.

**Bio, pins, website field** — profile page, instant, no commit required.

**SpendLens app** — any commit to `main` in that repo redeploys the live site automatically.

---

# Two things to settle before you start applying

**Make LinkedIn agree with the resumes.** LinkedIn says **Annalect India**; the resumes say
"Annalect India (Omnicom Group)". Your MBA start reads **April 2026** on LinkedIn. Pick one
version of each and make both places match — a recruiter will have both tabs open at once.

**Your other seven repositories.** Anything public with no README, a default name, or
abandoned starter code is one click away from your profile. Ten minutes to add a short README
or set them private. A recruiter who clicks "Repositories" and finds five empty ones draws a
conclusion you did not intend.
