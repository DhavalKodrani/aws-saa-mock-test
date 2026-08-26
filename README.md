# AWS Solutions Architect — Adaptive Mock Test

A free, single-page adaptive practice exam for the **AWS Certified Solutions Architect – Associate (SAA-C03)** exam. No build step, no dependencies — `index.html` plus one generated question file.

**▶ Live site:** https://dhavalkodrani.github.io/aws-saa-mock-test/

## Features

- **550+ question bank** across 3 difficulty levels: 🟢 Basic, 🟡 Intermediate, 🔴 Advanced
  - 90 hand-written questions (30 per level)
  - 466 questions imported from a community SAA-C03 exam dump (see note below)
- **Adaptive progression** — after each 20-question test:
  - **≥ 70%** → move **up** a level
  - **50–69%** → **stay** at the current level
  - **< 50%** → move **down** a level
- **Shuffled** questions *and* answer options on every test
- **Instant feedback** with a detailed explanation for every question (green = correct, red = wrong)
- **Progress bar** and running score during the test
- **Results screen** with a score ring, pass/fail verdict, and **category breakdown** (Architecture, Cost, Security, Database, Networking, Storage, Monitoring, Migration, Compute, Performance, Disaster Recovery)
- **Review mode** — expand any question after the test to re-read the scenario, your answer, the correct answer, and the explanation
- **Test history** and best score, saved in your browser (`localStorage`)
- **Keyboard shortcuts** — press `1`–`4` to answer, `←` / `→` to navigate
- **Mobile-responsive** dark UI

## About the imported questions

`questions-dump.js` is auto-generated from a community SAA-C03 exam dump. The dump provided each **question and its correct answer**, but not the wrong options. For those questions the three distractors were **generated automatically** from the pool of other questions' correct answers — they are plausible AWS solutions but are *not* authoritative, so treat wrong options and explanations as study aids and verify against the official AWS documentation. The 90 hand-written questions have fully authored options and explanations.

## Run locally

Open `index.html` in any browser — there is nothing to install. (Use a simple static server or GitHub Pages if your browser blocks the local `questions-dump.js` include under `file://`.)

## Deploy on GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source = Deploy from a branch**, **Branch = `main`**, **Folder = `/ (root)`**, then **Save**.
4. Your site goes live at `https://<username>.github.io/<repo>/` within a minute or two.

> Not affiliated with or endorsed by Amazon Web Services. For study purposes only.
