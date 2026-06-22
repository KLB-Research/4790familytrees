# Family Lifelines — PSYC 4790H

An interactive, single-file web tool for the Family Tree assignment in *Social Psychology of the Holocaust* (PSYC 4790H), Trent University.

Students enter the people in their family who were alive between roughly 1900 and 1950 and the page builds two timelines — a wide "in perspective" view and a 1933–1945 zoom — showing where their family sits in time relative to the Holocaust and to themselves.

## Live link

**https://klb-research.github.io/4790familytrees/**

Send students to that one URL. Nothing to install.

## Privacy

The page is a single static HTML file. It has no account, no server, and makes no network requests with student data — nothing a student enters ever leaves their own browser. Work is auto-saved to the browser's `localStorage` (on that device only) so they can close the tab and return later. The **Save my entries** button downloads a JSON backup file for moving between computers or guarding against cleared browser data.

## How students hand in their work

**Print / Save as PDF** is the deliverable. The PDF opens with an **APA 7 student title page** (built automatically from the student's name + number and the course details in CONFIG), followed by both timelines and the summary panels. **Download as images (PNG)** is also available for the two timelines on their own.

## Editing the assignment

Everything lives in `index.html` (HTML, CSS, and JavaScript in one file). Edit it, commit, and push — GitHub Pages redeploys automatically and the link stays the same.

**Routine changes (e.g. the due date each term):** edit the `CONFIG` block at the top of the `<script>` in `index.html`. It holds the assignment title, course code/name, department, institution, instructor, and **due date** — one line each. Change the `dueDate` line for the winter cohort and push:

```js
const CONFIG = {
  assignmentTitle: "Family Lifelines: A Holocaust-Era Family Timeline",
  courseCode:      "PSYC 4790",
  courseName:      "Social Psychology of the Holocaust",
  department:      "Department of Psychology",
  institution:     "Trent University",
  instructor:      "Dr. Karen L. Blair",
  dueDate:         "September 14, 2026"   // ← change this for the winter cohort
};
```

**Intro/instruction wording** lives in the page body (the `intro-text` section). **The historical events** on the timelines are the `EVENTS` array, just below `CONFIG`.

**Adding the logos:** in the `<div class="logos">` near the top of the body, replace the two placeholder `<span class="logo-placeholder">` chips with `<img>` tags pointing at logo files committed to this repo, e.g. `<img src="trent-logo.png" alt="Trent University">`.

To push changes: `git commit -am "…"` then `git push`. Or just ask Claude Code to make the change.

Maintained by KLB Research (SRAD Lab), Dr. Karen L. Blair.
