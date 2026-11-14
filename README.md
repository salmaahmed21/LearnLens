# LearnLens: AI-assisted assessment for Grades 1–5

CSEN 909 Human Computer Interaction, Winter 2026. Team **Five Stars**, Milestone 3 coded front-end (optional bonus).

LearnLens helps a teacher grade scanned handwritten exams. The system reads the answers (OCR) and suggests grades, learning gaps and red flags. **The teacher checks and approves every step**, and students only see results their teacher has published. This repository is a clickable HTML/CSS front-end of the full workflow, with simulated AI output. There is no back-end, as the course brief allows.

## Live demo
After GitHub Pages is turned on (see below), the demo is at:
`https://<your-github-username>.github.io/<repository-name>/`

## Run it locally (no installation needed)
1. Download the repository: green **Code** button → **Download ZIP**, then unzip it.
2. Double-click `index.html`. It opens in any web browser.
3. Choose a view: **Student**, **Teacher** or **Parent**. Every button and side-menu item is a working link.

Optional: run a local server with `python3 -m http.server 8000` in this folder, then open http://localhost:8000.

## Deploy with GitHub Pages
1. In the repository, open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, branch **main**, folder **/(root)**, and click **Save**.
3. Wait one or two minutes, then refresh the page. The live link appears at the top.

## What to try (main journey)
1. **Student (Omar):** Upload My Exam → Choose file → Continue to Preview → One last check! (page 1 and page 2) → Confirm & Submit → You did it! → View submission or Return to Dashboard.
2. **Teacher (Ms. Nehal):**
   1. Review Scan, click the flagged word "waiter", click Apply water correction, then Save corrections.
   2. Click Send for grading review.
   3. On Q4, click the mark to open Change the mark, set it from 4 to 3 with a reason, then click Save new mark. The total becomes 17 / 20.
   4. Click Review feedback, then Confirm flag on the red flag.
   5. Click Ready to share Omar's results?, then Publish Results.
3. **Student after results:** open the notification bell, then:
   1. Read the results, the feedback and the gently worded flag.
   2. Start Practice (Let's explore photosynthesis!), answer 3 questions, then Submit for Teacher Review.
   3. Look at My progress.
   4. Record a voice answer: big microphone, Pause recording or Stop and review, listen, Record again or Send to teacher.
   5. Teach it back!: Rehearse my explanation, listen, then send it.
4. **Teacher, more screens:**
   - Class Analytics: 24 students, averages by topic, the term trend, and students who may need support.
   - Voice: create a voice assessment (English or German), then review an answer with audio playback and transcript correction.
   - Edit the AI practice questions, and approve Omar's practice (Approve practice feedback).
   - Omar's German (Deutsch) exam: on the dashboard, click Review Scan on his Sachunterricht-Quiz row, fix the misread word "Wurtzeln" (his own spelling "Sonenlicht" stays), review the grade (14 / 16) and publish it. Omar then sees both results under Results & Feedback.
5. **Parent view:**
   - an overview, with notifications from the bell
   - all results, and one quiz question by question
   - progress over the term
   - Support at home: the teacher-confirmed flag explained, what school is doing, and tips
   - messages with the teacher
   - settings for notifications and language (English, Deutsch, Arabic)

## Structure
- `index.html`: the start screen
- `01_start.html` to `92_p_settings.html`: one self-contained page per screen. The CSS is inline and the icons are inline SVG ([Lucide](https://lucide.dev), ISC licence).

## Notes
- All names, grades and answers are fictional sample data.
- OCR, grading, flags and transcripts are hard-coded to simulate AI output.

## Screenshots
`docs/screenshots/` has a picture of every screen (01 to 92), in the same order as the pages.

## Put it on GitHub
1. On github.com, click **New repository**, give it a name (for example `learnlens-frontend`), make it **Public**, and click **Create repository**.
2. On the new page, click **uploading an existing file**.
3. Unzip this folder and open it. GitHub accepts up to 100 files per upload, so upload in two rounds:
   - Round 1: select all the files in the main folder (the `.html` files and `README.md`, not the `docs` folder), drag them into the browser window, and click **Commit changes**.
   - Round 2: click **Add file → Upload files**, drag the whole `docs` folder in, and click **Commit changes**.
4. Turn on GitHub Pages (see "Deploy with GitHub Pages" above) and add the live link to the submission.
