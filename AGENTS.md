# Repository Guidelines

## Mandatory Startup Rule

Before responding to any study request, read this `AGENTS.md` from the repository root. If it was not automatically loaded, read it manually before solving the question. Treat the learner context, explanation protocol, page references, and study progress below as required context for every session.

## Project Structure & Module Organization

This workspace is a flat collection of standalone scanned documents. The root contains nine numbered PDFs (`2101.pdf` through `2111.pdf`, with gaps) and one timestamped JPEG (`2026-09-14 18.38.59.jpg`). Keep original scans at the root unless a future organization scheme is documented. Store temporary renders under `tmp/pdfs/<paper>/`; store confirmed reference pages under `study-pages/<paper>/<unit>/` so they can be reused from another checkout.

Preserve supplied numeric filenames because they act as document identifiers. Name derived files with the identifier and a clear suffix, for example `2109-ocr.txt` or `2109-preview.png`; never overwrite the source scan.

## Build, Test, and Development Commands

No build system, dependency manifest, or automated test suite exists. Useful checks include:

```sh
file 2109.pdf
pdfinfo 2109.pdf
pdftotext 2109.pdf -
```

Use `file` for type, `pdfinfo` for page count and metadata, and `pdftotext` to check for an extractable text layer. Scanned PDFs may intentionally produce no text output.

## Coding Style & Naming Conventions

No programming language or formatter is configured. For documentation, use clear Markdown headings, short paragraphs, and fenced command examples. Keep original filenames unchanged. New filenames should use lowercase descriptive suffixes, hyphens, and the original numeric ID; avoid ambiguous names and spaces where practical.

## Testing Guidelines

Open changed files to confirm pages are complete, readable, and correctly oriented. Compare `pdfinfo` page counts with the source and check for truncation. Spot-check generated OCR or previews against the scan.

## Commit & Pull Request Guidelines

This checkout has no Git metadata or commit history, so project-specific commit conventions cannot be inferred. If version control is added, use concise imperative subjects such as `Add OCR output for 2109`, explain the document change in the body, and avoid committing temporary exports. Pull requests should describe affected filenames, validation performed, and any readability or OCR limitations; include before/after previews when visual changes matter.

## Security & Privacy

Treat scans and derived text as potentially sensitive. Do not upload them to external services or include secrets in metadata, OCR output, or examples. Keep originals intact and review generated files before distribution.

## Learner Context & Explanation Protocol

The learner has been away from school for about eight years and is now studying Second Year Mathematics without having taken First Year. Assume that most fundamentals, terminology, givens, question interpretation, theorems, and methods need rebuilding. Explain primarily in Burmese, from first principles: define terms and symbols, identify givens and unknowns, translate the question into a plan, explain why each theorem or method applies, show every calculation step, and point out common mistakes. Check understanding after each question. Never mark a question complete until the learner explicitly confirms understanding.

## Study Progress

AGENTS.md records selected questions and completion status. After explaining each question, update AGENTS.md immediately only when the learner explicitly confirms understanding. Confirmed reference pages are tracked in `study-pages/2103/unit-1/`: `page-02.png` (No. 5), `page-03.png` (No. 6-7), `page-05.png` (No. 10), and `page-06.png` (No. 11). Other renders remain local under `tmp/`.

- Paper 2103, Unit 1 — No. 5, 6, 7, 10, and 11: completed after learner confirmation.
- Additional foundation — Trigonometric ratios: studied SOH-CAH-TOA, the special-angle values for `0°, 30°, 45°, 60°, 90°`, and using `F cos θ` for horizontal components and `F sin θ` for vertical components. Detailed Burmese explanations are saved in [`study-notes/trigonometric-ratios.md`](study-notes/trigonometric-ratios.md). Retain for future review.
- English learning plan based on the `eng.pdf` exam format is saved in [`study-notes/english-learning-plan.md`](study-notes/english-learning-plan.md). Keep future English notes under `study-notes/` with the `english-` filename prefix; keep temporary renders under `tmp/pdfs/eng/` and confirmed reference pages under `study-pages/eng/<unit>/`.
- English — Reading Section I(a), reference words: completed after learner confirmation. Practised identifying what “This movement,” “It,” “them,” “These groups,” and “which” refer to in a passage.
- English — Reading Section I(b), matching: completed after learner confirmation. Practised matching paraphrased descriptions with the correct people or activities in a passage.
- English — Reading Section I(c), True / False: completed after learner confirmation. Practised deciding statements from passage evidence and noticing limiting words such as “all,” “completely,” and “some.”
- English — Reading Section I(d), answering passage questions: completed after learner confirmation. Practised answering why/how/result questions in complete sentences and correcting passive forms such as “could be saved.” Reading Section I is complete.
- English — Section III Word Forms foundation lesson: completed after learner confirmation. Practised choosing noun, adjective, adverb, and verb forms, including `refusal`, `improvements`, `useful/used`, and `enlarge`; Section III practice is ongoing.
- Paper 2109 — selected questions from the yellow-highlighted images: **Ex. 1.1**, **MQ No. 2 (Model Question)**, **S.A. 1.1 (2)(i)**, **S.A. 1.1 (1)**, **Ex. 1.2**, **No. 3**, the problem starting **“If `r = [x, y, z]`, prove that …”** (harmonic function), **No. 2** starting **“If `C` is a closed circuit …”**, and the problem starting **“Find the gradient of the function …”**. The first No. 2 is MQ; the later No. 2 is the closed-circuit problem. These are selected only and are not yet marked complete.
