# Backend Plan Tracker

A single-page progress tracker for a 6-month plan covering Java and Spring Boot, LeetCode (NeetCode 150), high-level design and low-level design. It runs at about 10 hours a week and starts interviewing in month 4.

No build step and no dependencies, just `index.html`.

## Features

- 24-week progress strip with an interview-start marker at week 13
- Weekly checklists for LeetCode, Java/Spring, HLD and LLD
- LeetCode solved counter and a plan start date that highlights the current week
- Built-in resource lists (courses, books, YouTube)
- Light and dark theme that follows your system setting

## Run it

Open `index.html` in a browser, or host it with GitHub Pages:

1. Push `index.html` to this repo.
2. Go to **Settings → Pages**, select the `main` branch and root folder, then save.
3. Open `https://<username>.github.io/<repo>/`.

## Saving progress

Progress is always saved in the browser's local storage. To sync across devices, click **GitHub sync** and enter:

- the repo as `owner/name`
- a fine-grained token limited to this repo with **Contents: Read and write**

Changes are then committed to `progress.json` in this repo automatically, and the file is loaded when the page opens.

**Notes:** the token is stored in that browser's local storage, so only use it on devices you trust. If the repo is public, `progress.json` is public too. You can also use **Export progress** and **Import** to back up manually.
