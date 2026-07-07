# Corporate Finance Leadership Interview Playbook

**Full-Time MBA Program · David Eccles School of Business**

A self-contained interview preparation tool for MBA candidates pursuing corporate finance leadership roles. It combines a 100-question interview bank, six core finance frameworks, and an AI-assisted practice studio with voice recording, instant scoring, and a readiness dashboard that tracks your progress over time.

---

**Live Playbook ▶ [Intv Playbook – Corporate Finance (vG)](https://coryjburk.github.io/intv-playbook-corp-finc_vc/)**

_The entire application is a single HTML file. There is no build step, no server, and no account — it runs completely in your browser, and your practice data never leaves your device._

---

## Quick Start

Open `cf-playbook.html` in a modern browser (Chrome or Edge recommended for voice practice), or visit the hosted version on GitHub Pages. Click **Question Bank** in the sidebar, pick a question, and press **🎤 Practice in Studio**. Speak or type your answer, submit it for evaluation, and watch your Readiness Dashboard build as you practice.

That's the whole workflow. The rest of this manual explains what each part does and how the scoring works.

---

## The Three Sections

**Readiness Dashboard** is the home screen. It shows your overall readiness score, per-competency progress bars (Financial Modeling & Valuation, Strategic Finance, Communication & Pacing), and performance logs including total attempts, average filler words, average self-assessment, and your recent trend.

**Question Bank** holds all 100 questions across 9 categories — Valuation, Accounting & 3-Statement, M&A & Corporate Development, Financial Modeling, Capital Allocation & Corp Finance, FP&A & Strategic Finance, Treasury, Markets & Risk, Strategy & Business Judgment, and Behavioral & Leadership. Two filter rows let you narrow by topic and by difficulty tier (Foundational → Core → Advanced → Expert). Each card offers a **Conversational** answer (how you'd say it aloud) and a **Deep Dive** (the full technical structure). Behavioral questions carry a CARL tag and are coached on story structure instead of keywords.

**Finance Frameworks** contains six reference frameworks — the 3-statement linking blueprint, DCF build order, WACC components, LBO value-creation levers, the capital allocation hierarchy, and the plan-vs-actual variance bridge — each broken into the steps you should be able to recite cold.

---

## The Practice Studio

Opening a question in the studio gives you a transcript area and two ways to answer. Click **🎤 Start Recording** to speak (the browser will ask for microphone permission the first time) or simply start typing. A timer starts on your first keystroke or the moment recording begins, so reading time doesn't count against you. When you're done, press **🧠 Submit for AI Evaluation**. Answers under 30 characters are rejected as too short to score meaningfully.

The results panel shows your score (0–100), word count, keyword or CARL-beat coverage, filler-word count, answer duration, and — for spoken answers only — your pace in words per minute. Typed answers deliberately show no WPM, because typing speed is not interview pacing. The pacing notes flag answers that run faster than ~170 WPM (rushed), slower than ~110 WPM (dragging), or longer than 2½ minutes (most interview answers should land in 60–120 seconds).

Below the score, two follow-up tools do the real coaching work:

**Get real AI feedback.** The built-in score checks keyword coverage and pacing — it cannot judge whether your reasoning is correct. The studio therefore generates a ready-made coaching prompt containing the question, the model framework, and your transcript. Copy it and paste it into Claude (the **Open Claude ↗** button opens a new chat) for substantive feedback on accuracy, structure, and a tightened version of your answer you could deliver aloud.

**Compare against the model answer.** Reveal how a strong candidate frames the question, then rate your own answer from 1 (major gaps) to 4 (strong). The tool compares your self-rating against your coverage score and tells you whether you're well calibrated, overconfident, or underselling yourself — a self-awareness signal interviewers actively probe for.

---

## How Scoring Works

The score measures *coverage and delivery*, not correctness. It is a practice heuristic, not a grade — use the AI coaching prompt for substance.

**Technical questions** start from a base of 30 points, add up to 30 points for answer length (full credit at ~80 words), add up to 40 points for hitting the finance concepts an interviewer listens for (6 points each), and subtract 3 points per filler word ("um," "like," "you know," and similar). Scores are capped at 0–100.

The keyword matcher is voice-aware: spoken transcripts never contain slashes, ampersands, or hyphens, so saying "EV to EBITDA," "SG and A," "P E ratio," or "sum of the parts" correctly matches keywords written as `ev/ebitda`, `sg&a`, `p/e`, and `sum-of-the-parts`.

**Behavioral questions** are scored on the CARL structure instead: 25 points for each detected story beat — Context/Challenge, Action, Result, Learning — minus 2 per filler word, minus 10 if the answer runs under 40 words. This is a structure check (is the beat present?), not a quality judgment.

| Score band | Meaning |
|---|---|
| 90–100 | Excellent coverage and delivery |
| 75–89 | Solid — a concept or beat is thin |
| 60–74 | Developing — meaningful gaps |
| Below 60 | Rework the answer before your next attempt |

---

## The Readiness Dashboard, Explained

The dashboard is driven by your **recent** performance — the average of your last 3 attempts on each question — not your single best run. Your overall readiness score is the mean of those per-question recent averages, so it reflects where you are now and can go down if your recent attempts slip. Readiness levels are Emerging (below 60), Developing (60+), Interview Ready (80+), and Offer Ready (90+).

The **Recent Trend** indicator compares the average of your last 3 attempts against the 3 before them, across all questions: a swing of 4+ points shows as Improving or Slipping; otherwise you're Holding Steady. It needs at least 4 total attempts before it reports anything.

The **Communication & Pacing** bar blends your behavioral-question performance with a filler-word pacing score, so it responds both to CARL practice and to cleaning up verbal habits.

Question cards show a **Recent N** badge — the same last-3 average that feeds the dashboard.

---

## Saving, Moving, and Resetting Progress

Progress saves automatically to your browser's local storage after every attempt. Because storage is per-browser and per-device, three header buttons manage it:

**📤 Export** downloads your complete progress as `cf-playbook-progress.json`. **📥 Import** loads a previously exported file — you'll see a summary of what the file contains and must confirm before it *replaces* the progress on the current device. **🔄 Reset Progress** permanently wipes everything after confirmation.

Export/Import is also your safety net in two situations: moving between devices (export on your laptop, import on your desktop) and browsers that block local storage (private/incognito windows show a warning banner — export before closing the tab or your session is lost).

---

## Privacy

Everything runs client-side. Your recordings, transcripts, and scores are processed in your browser and stored only in your browser's local storage. Nothing is transmitted to any server. The one deliberate exception is the AI coaching prompt: *you* copy it and *you* paste it into Claude — nothing is sent automatically, and nothing leaves the page unless you take that action.

Voice recording uses your browser's built-in speech recognition. Depending on the browser, the audio may be processed by the browser vendor's speech service (this is how Chrome's speech recognition works); the playbook itself never stores or transmits audio.

---

## Browser Support & Troubleshooting

| Symptom | Cause | Fix |
|---|---|---|
| Record button disabled, note about unsupported browser | Browser lacks the Web Speech API (Firefox, some others) | Type your answer — scoring works identically — or use Chrome/Edge |
| "Microphone access was blocked" | Mic permission denied | Click the padlock/site-settings icon in the address bar, allow the microphone, and try again — or type instead |
| Yellow banner about local storage | Private/incognito mode or storage disabled | Progress won't survive a reload; use 📤 Export before closing |
| Voice cuts out on iPhone/iPad | iOS Safari's speech recognition is unreliable | Known platform limitation — type answers on iOS, or practice voice on a desktop browser |
| Dashboard score dropped after an update | Scores now reflect recent attempts, not best-ever | Working as intended — keep practicing and the recent average recovers |

---

## For Maintainers

**Deployment.** Upload `cf-playbook.html` to any static host. For GitHub Pages, commit it to the repository and it's live at the corresponding URL — no build pipeline required.

**Editing content.** All content lives in three constants near the top of the `<script>` block. `QUESTIONS` holds every question — each entry needs an `id`, `category`, `competency` (`modeling`, `strategy`, or `communication`), `difficulty`, `title`, `conversational` answer, `deepDive` answer, and (for technical questions) a `keywords` array; behavioral questions instead set `type: "behavioral"`. `FRAMEWORKS` holds the six framework cards. `SCORING` controls the point math (base score, length bonus, keyword points, filler penalty). Categories and filters render automatically from the data — adding a question in a new category creates the filter button for you.

**Storage format.** Progress is stored under the key `eccles_cf_playbook_v2` as JSON containing per-question attempt records (score log, best, recent average, self-ratings, filler history) plus a global history of the last 12 scores. Version 1 progress is migrated automatically on first load. Note for the v1→v2 transition: v1 scores were computed under a more generous formula, so migrated scores will read slightly high until a few new attempts wash them out.
