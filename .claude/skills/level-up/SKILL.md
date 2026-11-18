---
name: level-up
description: Move the project to GitHub and put the page online. Once per project.
disable-model-invocation: true
---

You can't click anything in their browser. Give one step at a time, say exactly what they should see, and wait for "done" before the next step. If a screen doesn't match, ask them to describe it or send a screenshot.

1. Check that version 1 works and is saved. If not, suggest finishing first.
2. Explain in three sentences: GitHub stores the project online and keeps every version. GitHub Pages turns the docs folder into a live link. On a free account the project is public, so anyone with the link can read the files, including notes and reviews.
3. Privacy check of every file that will be uploaded (CLAUDE.md, NOTES.md, HABITS.md, reviews/, docs/). List anything private and fix it with them before going on.
4. GitHub account: open github.com/signup in their normal browser. "Continue with Google" or Apple is fine. Their username will be in the page's link, so pick one they're happy to share. Verify the email.
5. Make their project from the template: open the template link in the brief's footer, click "Use this template", then "Create a new repository". Name it (for example my-page), choose Public, click "Create repository from template".
6. Update "Where it lives" in CLAUDE.md to "GitHub: <username>/<repo-name>" and set Session number for next time. (Ask permission like any file change.)
7. Upload: in the new repository click "Add file", then "Upload files". Drag in CLAUDE.md, NOTES.md, HABITS.md and the reviews and docs folders from this project folder. Don't upload versions or set-aside. Click "Commit changes".
8. Turn on the site: Settings, then Pages, then under "Build and deployment" choose "Deploy from a branch", branch main, folder /docs, Save. It can take up to ten minutes.
9. Their link is https://<username>.github.io/<repo-name>/ . Ask them to open it on their phone.
10. Connect GitHub to Claude: open claude.ai/code in the browser and follow the "connect GitHub" prompt. If it offers to install the Claude GitHub App, install it on this repository only.
11. Tell them: from now on, work in a new session with environment Cloud and this repository, on the computer or the phone. This folder on the computer is now the old copy. After this session, rename it to "my-page (old copy)" and don't build in it anymore.
12. Count this as level 2 in NOTES.md.
