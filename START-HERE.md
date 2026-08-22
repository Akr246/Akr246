# START HERE — GitHub profile upgrade

Three repositories to update. Browser only. About 25 minutes.

```
1-portfolio-repo/       →  Akr246.github.io               (site + case studies + PROJECTS.md)
2-profile-repo/         →  Akr246                         (profile README)
3-spendlens-repo/       →  spendlens-ai-spend-intelligence (replaces its README)
resumes-to-apply-with/  →  keep on your computer
```

**What changed in this version**

- New **case studies page** — three deep dives with the reasoning, the trade-offs, and one thing that went wrong
- **"Actively interviewing"** status on the hero
- **Focus areas** keyword band — real ATS terms, visible rather than hidden
- **"Why React and TypeScript"** section added to the SpendLens card
- **PROJECTS.md** — a proper project index in the portfolio repo
- **Rewritten SpendLens README** — problem, role, architecture, decisions, what I'd change
- **Last updated** stamp in the footer

---

## PART 1 · Portfolio repo — `Akr246.github.io`

**Add file → Upload files.** Drag in **all five items** from `1-portfolio-repo`:

- `index.html` *(replaces the old one)*
- `case-studies.html` *(new)*
- `PROJECTS.md` *(new)*
- `assets` folder
- `resumes` folder

**Commit changes.**

Uploading a file with the same name replaces it — that is how `index.html` updates.

**Check:** open `https://akr246.github.io` and click **Case studies** in the hero. It should
load the new page. Also confirm the **Focus areas** band appears under the four numbers.

> If the folders do not come across, upload `assets` and `resumes` separately. This is the
> step that has failed before.

---

## PART 2 · Profile repo — `Akr246`

Open `README.md` → **pencil icon** → select all, delete → paste `2-profile-repo/README.md`
→ **Commit changes**.

**Check:** `github.com/Akr246` now shows the Focus areas line and links to Case studies and
PROJECTS.md.

---

## PART 3 · SpendLens repo — `spendlens-ai-spend-intelligence`

Open its `README.md` → **pencil icon** → select all, delete → paste
`3-spendlens-repo/README.md` → **Commit changes**.

This one matters more than it looks. Anyone who clicks through from your portfolio lands
here, and the old README was written before the case study existed.

---

## PART 4 · Two things only you can finish

The case studies page has **three `Fill this in` boxes** in mauve. They are in case studies
two and three — the Align Technē automation and the Annalect A/B test.

I wrote those two from your LinkedIn, which gives the outcome but not the working. The boxes
ask for the detail only you have:

- How often the billing cycle ran, and how long extraction took before and after
- Whether the 20% was measured on time, cost, or error rate
- What the A/B test's primary metric was and roughly how long it ran
- One honest "what I'd do differently" for each

**Edit them in `case-studies.html`** — search for `class="fill"`, replace the text between
the `<div>` tags, commit. Or delete the box entirely if you would rather leave the section short.

**Do not publish those two case studies with the boxes still visible.** A recruiter reading
"Fill this in" is worse than a shorter case study. Either complete them or remove the boxes.

---

## PART 5 · Profile settings, if not already done

**github.com/Akr246 → Edit profile**

Bio:
```
Psychology → product. I turn loose requirements into things teams can build. Ex-TPM @ Align Technē. MBA in AI for Business, in progress. Open to Product / BA / APM roles.
```

Website: `https://akr246.github.io` · Location: `Bengaluru, India` · Company: Alignerr or blank

**Customize your pins** → tick `spendlens-ai-spend-intelligence`, untick `testrepo`.

---

## Final check

- [ ] akr246.github.io loads and the **Case studies** button works
- [ ] Focus areas band visible under the stats
- [ ] "Actively interviewing" shows in the hero
- [ ] SpendLens repo README is the new one
- [ ] PROJECTS.md opens from the profile README
- [ ] **No `Fill this in` boxes remain visible on the published case studies page**
- [ ] Open the site on your phone

---

## What I did not build, and why

The advice you pasted suggested several things I have deliberately left out:

**Press mentions, speaking engagements, published articles, LinkedIn recommendations,
open-source contributions.** You do not have these yet. Adding them would be inventing a
record, which is the same problem as the sixteen projects — and these are all trivially
checkable.

**Star counts on repos.** Yours are at zero. Displaying that number draws attention to it.

**A Tableau dashboard link.** You built dashboards at Annalect, but that work belongs to
them. Do not publish it. If you want a public dashboard, build one on open data — that is
project 2 in the briefs document.

Three of those become available the moment you finish a project or two: an article about
the behavioural teardown, a public dashboard from the review-mining project, and a real
open-source repo. That is the honest route to the same outcome.
