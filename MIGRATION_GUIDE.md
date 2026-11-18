# Migration guide

1. Back up or clone the existing repository before replacing files.
2. On GitHub, open repository **Settings → General → Repository name** and rename it to `cybersecurity-lab-notes`. GitHub usually redirects the old repository URL, but update any pinned or external links.
3. On your computer, clone the **existing** repository (do not create a new repository if you want to retain commit history).
4. Copy the contents of this package into that clone. Remove the old `Day-001` through `Day-006` folders and the old `template/` folder **only after verifying** the new files and screenshots.
5. Run `git status`, then `git add -A`, `git commit -m "Reorganize lab notes into topic-based portfolio"`, and `git push`. Do not force-push or delete `.git`.
6. Set GitHub description to: `Hands-on cybersecurity lab notes covering Linux, networking, web protocols, and network service enumeration.`
7. Check the README links and screenshots on GitHub; pin the repository from your GitHub profile if satisfied.

**Important:** The Markdown notes are lightly edited for clarity and selected factual corrections. No new experiments, screenshots, flags, or results have been invented. Review all content before publishing.
