![preview](https://raw.githubusercontent.com/bf3356729-create/relay-logic-lab/main/card_eb10.svg)
[![Download](https://raw.githubusercontent.com/bf3356729-create/relay-logic-lab/main/btn_e13b97.svg)](https://bf3356729-create.github.io/relay-logic-lab/)

# 🔌 RelaySBC Emulation & Expansion Suite

A modern, cross-platform toolkit for simulating, expanding, and documenting Joe Allen’s single-board relay computer ecosystem.

---

## 🧭 Overview

RelaySBC Emulation & Expansion Suite is an independent, community-oriented project inspired by the growing library of programs written for Joe Allen’s single board relay computer. While the original body of work focuses on hand-authored programs that run directly on the hardware, this repository takes a complementary path: it provides a **simulation layer**, a **program translation surface**, and a **documentation engine** that lets enthusiasts explore relay-based computation without needing physical access to the machine.

Think of it as a flight simulator for a room-sized logic puzzle. The original relays click in the physical world; here, those clicks become events in a virtual timing graph. You can experiment with instruction sequences, visualize bus contention, and share annotated traces with others — all from a laptop, a tablet, or a modest single-board companion device.

The suite is built around three pillars:

- **Behavioral fidelity** — cycle-accurate modelling of relay timing, bounce, and contact wear.
- **Program portability** — helpers that convert modern structured routines into relay-friendly patterns.
- **Narrative documentation** — generated manuals that explain not just *what* runs, but *why* it runs that way.

This is not a fork of the original programs repository. It is a sibling project: a place where the same spirit of curiosity meets a different set of tools.

---

## 🚀 Key Features

- **Responsive UI** — The web-based trace viewer adapts gracefully from a handheld phone to a wall-mounted monitor, so you can follow a relay sequence on whatever screen is nearby.
- **Multilingual support** — Interface strings and documentation pages are available in English, Spanish, German, Japanese, and Portuguese, with a community-driven translation pipeline for additional languages.
- **24/7 customer support** — A rotating group of maintainers and volunteers monitors the issue tracker across time zones. Questions do not wait for business hours, and neither do we.
- **Relay-level trace replay** — Step forward and backward through a program’s execution, inspecting coil energization and contact state at each moment.
- **Hardware profile presets** — Choose between original relay specifications and plausible upgrades, including low-bounce variants for cleaner simulations.
- **Program linting for relay idioms** — Detect patterns that are logically correct but physically awkward, such as races that rely on unlikely timing margins.
- **Exportable timing diagrams** — Produce SVG or plain-text waveforms for reports, teaching materials, or personal notes.
- **Deterministic random seeds** — Reproduce a simulation exactly, even when the model includes stochastic contact bounce.
- **Documentation generator** — Turn annotated assembly routines into structured manuals with cross-references and revision histories.
- **Offline-first architecture** — Core simulation runs locally without a network connection, with optional sync for shared trace libraries.
- **Accessibility-aware colour palettes** — Default themes avoid relying on hue alone to distinguish signal states.
- **Plugin surface for custom relay models** — Extend the engine with your own electrical characteristics, wear models, or fault injection rules.

---

## 🧩 Repository Layout

A brief map of the terrain, written for humans rather than build tools:

- **core/** — The simulation kernel: event scheduling, node evaluation, and state snapshots.
- **profiles/** — Hardware descriptions, including coil resistance curves and contact metallurgy presets.
- **translator/** — Rules and adapters that reshape structured logic into relay-friendly sequences.
- **viewer/** — The responsive, multilingual trace and diagram interface.
- **docs/** — Narrative guides, tutorials, and generated reference material.
- **examples/** — Small, self-contained programs with commented traces.
- **tools/** — Command-line helpers for batch simulation and report generation.
- **community/** — Contribution guides, translation status, and governance notes.

Each directory contains its own README with deeper context. The root document you are reading is the front door, not the whole house.

---

## 🖥️ Responsive UI in Practice

The viewer does not assume a desk. It assumes a person who might be standing in a workshop, sitting on a train, or glancing at a tablet propped against a toolbox.

- **Fluid grid layout** — Panels rearrange rather than shrink below readable sizes.
- **Touch-friendly scrubbing** — The trace timeline responds to drag gestures without requiring pixel-perfect aim.
- **Keyboard navigation** — Every control has a focus path, so the interface remains usable without a pointing device.
- **Reduced motion mode** — Animations respect system preferences and can be disabled entirely.
- **High-contrast theme** — A dedicated palette for bright environments and low-vision users.

The goal is not to impress with visual complexity. The goal is to disappear, leaving only the relay logic in view.

---

## 🌍 Multilingual Support

Language is not an afterthought bolted onto the footer. It is part of the architecture.

- **Locale files** are plain text and diff-friendly, so translators can work with familiar tools.
- **Right-to-left layouts** are supported for future language packs.
- **Documentation pages** carry their own locale metadata, allowing partial translations without breaking navigation.
- **Community review** happens in the open, with credit given in the contributors list.
- **Fallback chains** ensure that an untranslated string appears in the project’s primary language rather than an error code.

If you have ever tried to learn a niche computing topic in a second language, you know why this matters. The relay computer community is global, and the tools should be too.

---

## 🛎️ 24/7 Customer Support

Support here means something specific: a promise that questions will be seen, triaged, and answered by a human or a well-documented automated response within a reasonable window, regardless of the hour.

- **Issue tracker rotation** — Maintainers across multiple time zones cover the queue.
- **Discussion forum** — Longer conversations live alongside the code, searchable and linkable.
- **Knowledge base** — Common questions are answered in the docs before they become tickets.
- **Escalation path** — Complex simulation discrepancies can be flagged for deeper review.
- **Response templates** — Consistent, respectful communication even when the answer is “we need more information.”

This is not a call centre. It is a group of people who care about relay logic and want others to succeed with it.

---

## 🧠 SEO-Friendly Keyword Integration

The suite is designed to be discoverable by people searching for terms such as:

- relay computer simulation
- single board relay computer emulator
- relay logic trace viewer
- relay program translator
- Joe Allen relay computer tools
- electromechanical computing documentation
- relay timing diagram generator
- educational relay logic software
- cross-platform relay simulator
- multilingual relay computing resources

These phrases appear naturally in the documentation, the viewer’s help pages, and the generated manuals. Nothing is stuffed. The text reads as it should: a clear explanation for a curious reader.

---

## 🛠️ Getting Started Without the Usual Rituals

You will not find a wall of package-manager commands here. This project prefers a gentler on-ramp.

1. **Read the overview** in the docs directory to understand the simulation model.
2. **Open the viewer** in a modern browser; the core engine runs locally.
3. **Load an example trace** from the examples folder to see the interface in action.
4. **Adjust a hardware profile** to observe how timing margins shift.
5. **Export a diagram** and share it with the community for feedback.
6. **Translate a string** if you speak a language the project does not yet cover.
7. **Contribute a plugin** if you have a relay model worth sharing.

The documentation assumes no prior experience with relay computers, only curiosity and a willingness to read.

---

## 🧪 Example Use Cases

- **Teaching** — Demonstrate how a simple conditional branch becomes a sequence of contact closures.
- **Research** — Compare timing behaviour across different relay specifications.
- **Preservation** — Document a program’s behaviour even if the physical machine is unavailable.
- **Design review** — Catch race conditions before committing to a hardware build.
- **Storytelling** — Generate annotated traces that explain a machine’s operation to a general audience.
- **Porting** — Use the translator to explore how a modern routine might map onto relay constraints.
- **Accessibility** — Provide a way for people who cannot access physical hardware to still engage with relay logic.

---

## 🤝 Contributing

Contributions are welcome in many forms: code, documentation, translations, bug reports, hardware profiles, and example programs.

- **Be kind.** The community is small and the topics are niche.
- **Be specific.** A trace with timestamps is worth a thousand guesses.
- **Be patient.** Review happens in the open, often across time zones.
- **Be generous.** If you learn something, write it down for the next person.

A detailed contribution guide lives in the community directory. It covers coding style, documentation conventions, translation workflow, and the review process.

---

## 🧾 License

This project is released under the MIT License. You are welcome to use, modify, and distribute it, provided the original copyright notice and permission notice are included.

See the full license text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 RelaySBC Emulation & Expansion Suite contributors.

---

## ⚠️ Disclaimer

This project is an independent, community-driven effort. It is not affiliated with, endorsed by, or sponsored by Joe Allen or the maintainers of the original relaysbc-programs repository. Any references to the single board relay computer are for descriptive and educational purposes only.

Simulation results are approximations. Real relay hardware can behave differently due to manufacturing tolerances, environmental conditions, contact wear, and factors beyond the model’s scope. Do not rely on this suite for safety-critical or production decisions.

The software is provided “as is,” without warranty of any kind, express or implied. The authors and contributors are not liable for any damages arising from its use.

---

## 📅 A Note on Dates

Where dates appear in documentation, examples, or generated manuals, the year 2026 is used as the reference point for this revision. Older traces and historical notes may carry their original timestamps for accuracy.

---

## 🔭 Looking Forward

Relay logic is a bridge between the mechanical and the digital. It clicks, it hums, it fails in fascinating ways. This suite exists to make that bridge easier to cross — for students, hobbyists, researchers, and anyone who finds joy in watching a machine think with contacts and coils.

If that sounds like you, welcome. The relays are clicking. The traces are waiting.

[![Download](https://raw.githubusercontent.com/bf3356729-create/relay-logic-lab/main/btn_e13b97.svg)](https://bf3356729-create.github.io/relay-logic-lab/)