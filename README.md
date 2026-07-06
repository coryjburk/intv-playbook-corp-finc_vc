# 📊 Corporate Finance Leadership Interview Playbook
**Full-Time MBA Program · David Eccles School of Business**

> A self-contained, browser-based practice tool for MBA candidates preparing for **Corporate Finance, Strategic Finance, and FP&A leadership interviews.** Built for the University of Utah David Eccles School of Business MBA program.

---

**▶ [Launch the Playbook][https://coryjburk.github.io/intv-playbook-corp_finc-vg-/]**

---

A 100-question bank paired with a practice studio that scores your spoken or typed answers, generates a tailored AI coaching prompt, lets you self-assess against model answers, and tracks your readiness over time. It's a single HTML file with no dependencies and no build step — open it locally or deploy it to GitHub Pages as-is.

---

## Features

- **100 questions** across **9 categories** and **4 difficulty tiers** (Foundational → Core → Advanced → Expert).
- **Practice studio** with speech-to-text dictation or typing, plus instant scoring.
- **Two scoring engines** — keyword coverage for technical questions, and the **CARL** framework (Context · Action · Result · Learning) for behavioral questions.
- **AI Coaching Prompt generator** — one click builds a prompt (question + model framework + your answer) to paste into Claude for real feedback on quality and correctness.
- **Model-answer reveal** with a **1–4 self-score** and a calibration note that compares how you rated yourself to the keyword evidence.
- **Readiness Dashboard** with competency bars and performance logs, saved locally on your device.
- **Topic + difficulty filters** that combine, with a live result count.
- **Single file, no build, GitHub Pages-ready.**

---

## Table of Contents

- [Quick Start](#quick-start)
- [The Three Sections](#the-three-sections)
- [The Question Bank](#the-question-bank)
- [The Practice Studio](#the-practice-studio)
- [How Scoring Works](#how-scoring-works)
- [AI Coaching Prompt](#ai-coaching-prompt)
- [Model Answer and Self-Scoring](#model-answer-and-self-scoring)
- [The Readiness Dashboard](#the-readiness-dashboard)
- [Things You Might Notice (and Why)](#things-you-might-notice-and-why)
- [Tips for Best Results](#tips-for-best-results)
- [Troubleshooting](#troubleshooting)
- [Deployment](#deployment)
- [Repository Structure](#repository-structure)
- [Editing the Question Bank](#editing-the-question-bank)
- [Tech Notes](#tech-notes)
- [About](#about)

---

## Quick Start

1. Open the tool in **Chrome or Edge** (see the speech note under [Things You Might Notice](#things-you-might-notice-and-why)).
2. Click **Question Bank** in the left sidebar.
3. Pick any question and read the answer tabs to learn the structure.
4. Click **Practice & Grade Answer**, then speak or type your own answer.
5. Click **Submit for AI Evaluation** for a score, a keyword (or CARL) breakdown, a copy-ready AI coaching prompt, and the option to reveal the model answer and rate yourself.
6. Check the **Readiness Dashboard** to watch your progress build over time.

Your progress saves automatically on the device you're using.

---

## The Three Sections

The left sidebar has three areas:

- **Readiness Dashboard** — your overall readiness score, competency breakdown, and practice logs.
- **Question Bank** — all 100 questions, filterable by topic and difficulty.
- **Finance Frameworks** — six core structured-thinking blueprints (3-statement linking, DCF build order, WACC components, LBO value levers, capital allocation hierarchy, variance bridge) to know cold.

---

## The Question Bank

### Filtering

Two filter rows work together:

- **Topic** — the nine categories, from Valuation and Accounting to Behavioral & Leadership.
- **Difficulty** — Foundational, Core, Advanced, Expert.

Selecting one from each row narrows the list to the intersection (for example, *Advanced + Valuation*). A live "Showing X of 100 questions" count sits above the cards, and an empty combination shows a short message rather than a blank screen.

### Reading a question card

Each card shows the category, a color-coded difficulty tag, the question, and two answer tabs:

- **Technical questions** show a **Conversational Answer** (a tight, interview-ready response) and a **Deep Dive** (the framework and nuance behind it).
- **Behavioral questions** carry a green **CARL** tag and show a **Model Answer** and a **CARL Breakdown** (guidance on each storytelling beat).

Once you've practiced a question, a green **Best XX** badge appears showing your highest score for it.

### Difficulty color key

| Tier | Meaning |
|---|---|
| 🟢 **Foundational** | Definitional must-knows everyone should answer cold |
| 🟡 **Core** | Standard questions you'll reliably get |
| 🟠 **Advanced** | Multi-step synthesis and judgment |
| 🔴 **Expert** | Open-ended, senior-level judgment calls |

---

## The Practice Studio

Click **Practice & Grade Answer** on any card to open the studio.

- **Type** your answer in the box, or click **Start Recording** to dictate it.
- Click **Submit for AI Evaluation** when you're done — the microphone turns off automatically on submit.

After you submit, the results panel shows a **score** (0–100, color-shifted by tier), three metrics — **Words**, **Keywords Hit** (or **CARL Parts** for behavioral), and **Filler Words** — and a breakdown of which keywords you mentioned and which to work in, or for behavioral questions, a checklist of which CARL beats you landed.

> **Note:** Answers shorter than about 30 characters are declined with a prompt to give a fuller response — the scorer needs something real to evaluate.

---

## How Scoring Works

The in-app score is a fast, transparent **heuristic** — not an AI judgment of whether your answer was *correct*. It rewards completeness and clean delivery. Here's the exact math.

### Technical questions

Starts at a base of 50, then:

| Factor | Effect |
|---|---|
| Length | Up to **+25**, scaling to a maximum at ~80 words |
| Keywords | **+6** per core concept mentioned, capped at +30 (≈5 hits) |
| Filler words | **−3** each ("um," "like," "basically"…) |

Clamped to 0–100. Your **best** score per question is what's saved.

### Behavioral questions (CARL)

Behavioral questions are scored on **structure**, not keywords. The tool checks whether each of the four CARL beats is present:

- **C** — Context / Challenge
- **A** — Action (what *you* did)
- **R** — Result (the outcome, ideally quantified)
- **L** — Learning (the reflection)

Each beat present is worth **25 points** (4 beats = 100), minus a light filler penalty and a small deduction for very short answers. The score literally tells you how many of the four beats you landed.

---

## AI Coaching Prompt

Because the score above can't judge *quality or correctness*, every practice session generates a ready-to-use **AI Coaching Prompt** that already contains the question, the model framework, and your transcribed answer.

- Click **Copy Coaching Prompt**, then **Open Claude** to paste it into a fresh chat.
- For technical questions, the AI grades your reasoning and models a stronger version.
- For behavioral questions, it evaluates your answer beat-by-beat against CARL.

This is where you learn whether your answer was actually **good** — the in-app score only tells you whether it was **complete**.

---

## Model Answer and Self-Scoring

Below the coaching prompt, click **Reveal Model Answer** to see how a strong candidate would frame the question. It stays hidden until after you submit, on purpose — so you commit to your own answer first.

Then rate yourself **1–4**:

| Rating | Meaning |
|---|---|
| **1** | Major gaps |
| **2** | Partial |
| **3** | Solid |
| **4** | Strong |

The tool then shows a **calibration note** comparing your self-rating to the keyword score. Rate yourself higher than the coverage suggests and it nudges you to actually *say* the frameworks out loud; rate yourself lower and it points out the substance was there and the issue is likely delivery. Good calibration — your honest self-read matching the evidence — is exactly what holds up in a real interview.

---

## The Readiness Dashboard

- **Overall Readiness Score** — the average of your best score across every question practiced, with a tier label.
- **Competency Averages** — three bars: *Financial Modeling & Valuation* and *Strategic Finance* average your best scores in those skill areas, while *Communication & Pacing* blends your filler-word rate with your behavioral CARL scores.
- **Performance Logs** — questions practiced (out of 100), total attempts, average filler words, average self-assessment (out of 4), and a recent trend indicator.

### Readiness tiers

| Score | Tier |
|---|---|
| — | Not Evaluated |
| 0–59 | Emerging |
| 60–79 | Developing |
| 80–89 | Interview Ready |
| 90–100 | Offer Ready |

**Reset Progress** (top right) wipes everything after a confirmation step.

---

## Things You Might Notice (and Why)

These are deliberate design choices, not bugs. Knowing them up front will save confusion.

| What you'll notice | Why it works that way |
|---|---|
| **The microphone doesn't work in some browsers.** | Speech recognition uses a browser feature available in **Chrome and Edge** but not Firefox or some others. When it's unavailable, the mic button is disabled with a note — just type your answer. Scoring works identically either way. |
| **Your progress doesn't follow you to another device or browser.** | Progress is saved **locally on the device and browser** you're using, not to an account or the cloud. Practicing on your laptop won't appear on your phone, and clearing browser data resets it. This keeps the tool free, private, and login-free. |
| **A keyword-stuffed answer can score high; a great answer phrased unusually can score lower.** | The in-app score checks whether the right **concepts appear**, not whether you used them correctly. It measures *completeness*, not *quality* — which is exactly why the **AI Coaching Prompt** exists. Paste it into Claude for the real judgment on correctness. |
| **"AI Evaluation" isn't actually calling an AI.** | The instant score is a local heuristic, so it's fast and works offline. The genuine AI feedback is the **copy-to-Claude prompt** — that's the part powered by a real model. |
| **The CARL checker sometimes says a beat is "missing" when you feel you covered it.** | It detects each beat by recognizing signal language — past-tense first-person verbs for *Action*, quantified outcomes for *Result*, phrases like "I learned" for *Learning*. If you implied a beat without clearly stating it, it may not register. It errs toward telling you to **state the beat explicitly**, which is good interview habit anyway. |
| **The "Communication & Pacing" bar only moves after you practice — and reflects more than just talking.** | It blends your filler-word rate with your behavioral CARL scores, so it stays at zero until you've practiced and grows as both your delivery and storytelling improve. |
| **Re-practicing a question doesn't inflate your "questions practiced" count.** | The count tracks **unique** questions. Re-doing one updates your *best* score and adds to *total attempts*, but you still count as one question practiced — so the dashboard reflects breadth honestly. |
| **Your self-rating and the keyword score are shown side by side, not merged.** | Two honest signals you can compare tell you more than one blended number that hides the disagreement — and the disagreement (e.g., "I felt strong but missed the keywords") is where the learning is. |
| **Only your best score per question sticks.** | The dashboard rewards your demonstrated ceiling, so a rough first attempt won't permanently drag down your readiness once you nail the question later. |
| **The model answer stays hidden until you submit.** | This is on purpose — committing to your own answer first makes the comparison meaningful and prevents passive "read the answer, feel ready" practice. |

---

## Tips for Best Results

- **Practice out loud.** Typing tests your knowledge; speaking tests delivery and pacing — what the interview actually measures.
- **Treat the score as a completeness check, then use the AI prompt for quality.** The two together are far more useful than either alone.
- **Rate yourself honestly,** then read the calibration note. Closing the gap between how good you *feel* and how good you *are* is the whole game.
- **Work the Expert and Advanced tiers last,** once the Foundational and Core mechanics are automatic.
- **Use the Frameworks section** as a warm-up before a modeling or valuation block.

---

## Troubleshooting

| Symptom | Likely cause / fix |
|---|---|
| Mic button is greyed out | You're not in Chrome or Edge. Type your answer, or switch browsers. |
| Progress disappeared | Browser data was cleared, or you're on a different device/browser. Progress is device-local by design. |
| Score seems too low for a good answer | The scorer checks keyword/CARL presence, not quality. Make sure you're *saying* the core concepts; use the AI prompt for a real assessment. |
| "Answer too short" message | Give a fuller response — the scorer needs at least a sentence or two. |
| Nothing happens on Submit | Make sure there's text in the box and it's longer than a few words. |

---

## Deployment

This is a static site — no server, no build step.

1. Create a **public** repository (e.g., `cf-interview-playbook`).
2. Add the playbook HTML file to the repo root and rename it **`index.html`** for a clean URL.
3. Go to **Settings → Pages**, set the source to the **main** branch / **root** folder, and click **Save** (the Save step is required — Pages won't deploy without it).
4. Your tool will be live at `https://<username>.github.io/<repo>/` within a minute.

> Re-commits trigger a rebuild in under a minute. If you don't see an update, do a hard refresh (`Cmd/Ctrl + Shift + R`) to clear the browser cache.

---

## Repository Structure

| File | Purpose |
|---|---|
| `index.html` | The playbook (rename of the playbook HTML file). |
| `manual.html` | Optional branded in-app help page; link it from the playbook sidebar. |
| `README.md` | This document. |

---

## Editing the Question Bank

The entire bank lives in editable configuration objects at the top of the HTML file:

- **`QUESTIONS`** — each entry has `id`, `category`, `competency` (`modeling` / `strategy` / `communication`), `difficulty` (`Foundational` / `Core` / `Advanced` / `Expert`), `title`, `conversational`, `deepDive`, and either `keywords` (technical) or `type: "behavioral"` (CARL-scored, no keywords needed).
- **`FRAMEWORKS`** — the frameworks reference cards.
- **`SCORING`** and **`CARL`** — the scoring weights and behavioral detection patterns.

Adding a question is a copy-paste of one object; the hero counts, both filters, and the dashboard all update automatically from the array. To keep behavioral model answers scoring a clean 4/4, make sure each includes a clear Context cue, first-person past-tense Actions, a quantified Result, and an explicit "I learned…" Learning beat.

---

## Tech Notes

- **Stack:** plain HTML, CSS, and vanilla JavaScript in one file. No frameworks, dependencies, or build tooling.
- **Persistence:** browser `localStorage` (device-local), wrapped in error handling so it degrades gracefully to in-memory if a sandbox blocks storage.
- **Speech-to-text:** the Web Speech API (`webkitSpeechRecognition` / `SpeechRecognition`), available in Chromium-based browsers, with a typed-answer fallback everywhere else.
- **Design system:** University of Utah crimson (`#CC0000`) and gold (`#c9a84c`) on a dark theme, with the Inter typeface.
- **No tracking, no ads, no login.**

---

## About

Built for the **University of Utah David Eccles School of Business** MBA program as part of a suite of self-service career tools. Part of a family of single-file, GitHub Pages-deployed tools that share a consistent design system and editable configuration pattern.
