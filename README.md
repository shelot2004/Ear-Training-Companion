![preview](https://raw.githubusercontent.com/shelot2004/Ear-Training-Companion/main/banner_04d48.svg)
# 🎼 Interval-Trainer → Harmonic Compass

### A Distinct Repository Idea: **Aural Compass — Ear Training for the Wandering Musician**

**Repository:** DisturbingTheField/Aural-Compass

[![Download](https://raw.githubusercontent.com/shelot2004/Ear-Training-Companion/main/pkg_5063.svg)](https://shelot2004.github.io/Ear-Training-Companion/)

---

## 🧭 Overview

Aural Compass is the natural evolution of the humble interval trainer. Where Interval-Trainer taught you to recognize the distance between two notes, Aural Compass teaches you to *navigate* by ear — like a sailor reading the stars instead of a GPS. It is a lightweight, mobile-first web application that transforms the study of intervals, chords, scales, and rhythmic cells into an immersive auditory expedition.

Think of it this way: most ear-training tools hand you a flashlight and point it at a single note. Aural Compass hands you a compass, a sextant, and a star chart, then invites you to wander. Whether you are a conservatory student grinding through solfège, a bedroom producer training your ear for mix translation, or a hobbyist who simply wants to jam along with a record, Aural Compass adapts to your level and grows with you.

Built with a philosophy of progressive overload, spaced repetition, and generous feedback loops, this project aims to become the reference-grade open-source ear-training companion for the 2026 musician-on-the-move.

---

## 🎯 Why Another Ear Trainer?

Interval-Trainer proved that a small, focused web app can deliver real pedagogical value. Aural Compass takes the same spirit and expands it along three axes:

1. **Breadth** — intervals, chords, scales, modes, rhythmic subdivisions, and melodic dictation in one unified interface.
2. **Depth** — adaptive difficulty that responds to your actual accuracy, response time, and confidence.
3. **Warmth** — a deliberately calm, non-punishing interface that encourages repeated daily practice instead of gamified anxiety.

The result is less of a "quiz app" and more of a "practice room that fits in your pocket."

---

## ✨ Feature Highlights

### 🎧 Core Training Modules
- **Interval Recognition** — ascending, descending, harmonic, and compound intervals across all twelve chromatic roots.
- **Chord Quality Identification** — triads, sevenths, extensions, inversions, and voicings with configurable register.
- **Scale & Mode Recognition** — from major and natural minor through Dorian, Phrygian, Lydian, Mixolydian, Locrian, and exotic scales.
- **Melodic Dictation** — short melodies played back at adjustable tempo, with note-by-note grading.
- **Rhythmic Dictation** — tap or click subdivisions and receive instant rhythmic accuracy scores.
- **Perfect Pitch Drills** — optional pitch-class identification for those chasing absolute pitch.

### 🧠 Intelligent Practice Engine
- **Adaptive Difficulty** — the algorithm tracks your rolling accuracy and nudges the pool of questions toward your growth edge.
- **Spaced Repetition Scheduler** — intervals and chords you struggle with reappear more frequently; mastered ones fade gently into review.
- **Response-Time Awareness** — a slow-but-correct answer is weighted differently from a fast-but-correct one.
- **Session Summaries** — after every session, you receive a heat-map of strengths and blind spots.

### 📱 Responsive UI
- Designed with a mobile-first breakpoint system.
- Thumb-reachable controls for one-handed practice on a commute.
- Works beautifully on phones, tablets, laptops, and huge studio displays alike.
- Respects system dark/light preferences and offers a manual override.

### 🌍 Multilingual Support
- Interface strings externalized for easy translation.
- Currently shipping with English, Spanish, French, German, Japanese, and Brazilian Portuguese.
- Community translation workflow documented in the contributing guide.

### 🛠️ Developer-Friendly Architecture
- Zero-config build with modern bundler defaults.
- Pure Web Audio API for synthesis — no external sample dependencies required to get started.
- Pluggable question generators so that new drill types are drop-in additions.
- Typed core logic to reduce regressions as the feature surface grows.

### ☎️ 24/7 Customer Support
- A monitored issue tracker with a documented response window.
- Community chat channel for quick questions.
- Maintainer rotation ensures that even at 3 a.m. in your timezone, someone is watching the queue.

### 🎨 Accessibility
- Full keyboard navigation.
- Screen-reader-friendly ARIA labels on every interactive control.
- Adjustable contrast modes.
- Configurable audio feedback for users who cannot rely on visual grading alone.

### 🔒 Privacy by Design
- All practice data is stored locally in the browser by default.
- No account required to begin.
- Optional cloud sync is opt-in and uses end-to-end encrypted transport.

---

## 🚀 Getting Started

There are no terminal incantations required to try Aural Compass. Because it is a web application, the fastest path is to open the hosted build in your preferred browser, tap the start button, and let your ear do the walking.

[![Download](https://raw.githubusercontent.com/shelot2004/Ear-Training-Companion/main/pkg_5063.svg)](https://shelot2004.github.io/Ear-Training-Companion/)

For those who prefer to run it locally, the project is designed to be served from any static host. Point your local web server at the built output directory and navigate to the entry page. Nothing more exotic than that.

---

## 📚 SEO-Friendly Context: Who Is This For?

Aural Compass sits at the intersection of several search intents that musicians express every day. If you have ever typed any of the following into a search engine, this project was written with you in mind:

- "best ear training app for guitarists"
- "interval recognition practice online"
- "chord ear training for producers"
- "melodic dictation exercises for singers"
- "music theory practice tool for beginners"
- "adaptive ear training with spaced repetition"
- "mobile-friendly solfège trainer"
- "how to recognize scales by ear"
- "rhythm dictation practice for drummers"

The application is intentionally broad enough to serve classroom teachers, private instructors, self-taught learners, and working professionals who simply want to keep their ears sharp.

---

## 🏗️ Project Architecture

Aural Compass is organized into a small number of clearly separated layers, each of which can be reasoned about independently.

- **Audio Layer** — wraps the Web Audio API and provides a stable interface for note playback, chord construction, and rhythmic scheduling.
- **Theory Layer** — a pure, dependency-light module that encodes intervals, scales, chords, and their relationships.
- **Generator Layer** — produces question objects for each drill type. Each generator is registered against a difficulty profile.
- **Scheduler Layer** — handles spaced repetition, question selection, and adaptive difficulty adjustments.
- **UI Layer** — framework-agnostic components responsible for rendering, animation, and interaction.
- **Persistence Layer** — a thin abstraction over local storage with an optional remote adapter.

Each layer communicates through explicit contracts, which means that swapping out the UI framework or the audio backend would not disturb the theory or scheduler logic.

---

## 🧪 Testing & Quality

- Unit tests cover the theory and generator layers exhaustively.
- Integration tests exercise session flows end to end.
- Manual QA checklists are maintained for audio-specific behaviors that are hard to assert programmatically.
- A nightly pipeline runs the full suite against multiple browsers.
- Performance budgets are enforced so that the initial load stays lean.

---

## 🗺️ Roadmap

- **Q1 2026** — Public launch of core modules with six languages.
- **Q2 2026** — Native iOS and Android wrappers around the web build.
- **Q3 2026** — Instructor dashboard with class-wide progress analytics.
- **Q4 2026** — Community drill marketplace and shared lesson packs.
- **Beyond** — Real-time collaborative ear-training rooms, harmonic dictation, and transcriber assistance tools.

---

## 🤝 Contributing

Contributions are welcome and appreciated. Whether you fix a typo, add a translation, propose a new drill type, or refactor the scheduler, your work moves the project forward.

Before opening a pull request, please:

1. Read the contribution guidelines.
2. Run the test suite locally.
3. Keep changes scoped to a single concern.
4. Write commit messages that explain *why*, not just *what*.

First-time contributors are especially encouraged to look for issues tagged as beginner-friendly.

---

## 📜 License

Aural Compass is released under the MIT License. You are welcome to use, modify, and redistribute the code under the terms of that license.

Read the full license text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 DisturbingTheField

---

## ⚠️ Disclaimer

Aural Compass is an educational tool intended to support musical practice. It is provided "as is," without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement.

- The maintainers are not responsible for any hearing discomfort arising from extended headphone use. Please practice at sensible volumes and take regular breaks.
- Audio playback quality depends on the browser, operating system, and hardware of the listener. Results may vary across devices.
- Progress data stored locally may be lost if browser storage is cleared. Users who depend on long-term records should enable optional synchronization.
- Nothing in this project constitutes professional musical, medical, or pedagogical advice.

---

## 💬 A Closing Note

Ear training is not a sprint, and it is not a chore. It is a slow walk through a landscape that keeps revealing new paths the longer you stay. Aural Compass exists to make that walk pleasant, portable, and endlessly repeatable. Pick it up for five minutes on a bus, or lose yourself in it for an hour at a desk. Either way, your ears will thank you.

Happy listening, and may your intervals always resolve.

[![Download](https://raw.githubusercontent.com/shelot2004/Ear-Training-Companion/main/pkg_5063.svg)](https://shelot2004.github.io/Ear-Training-Companion/)