# Family Lifelines — PSYC 4790H

An interactive, single-file web tool for the Family Tree assignment in *Social Psychology of the Holocaust* (PSYC 4790H), Trent University.

Students enter the people in their family who were alive between roughly 1900 and 1950 and the page builds two timelines — a wide "in perspective" view and a 1933–1945 zoom — showing where their family sits in time relative to the Holocaust and to themselves.

## Live link

**https://klbresearch.github.io/4790familytrees/**

Send students to that one URL. Nothing to install.

## Privacy

The page is a single static HTML file. It has no account, no server, and makes no network requests with student data — nothing a student enters ever leaves their own browser. Work is auto-saved to the browser's `localStorage` (on that device only) so they can close the tab and return later. The **Save my entries** button downloads a JSON backup file for moving between computers or guarding against cleared browser data.

## How students hand in their work

- **Download as images (PNG)** — exports both timelines, or
- **Print / Save as PDF** — a print-formatted version of the timelines and summary panels.

## Editing the assignment

Everything lives in `index.html` (HTML, CSS, and JavaScript in one file). Edit it, commit, and push — GitHub Pages redeploys automatically and the link stays the same.

Maintained by KLB Research (SRAD Lab), Dr. Karen L. Blair.
