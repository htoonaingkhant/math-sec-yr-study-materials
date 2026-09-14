# Repository Guidelines

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

- Paper 2103, Unit 1 — No. 5, 6, and 7: completed after learner confirmation. No. 10 and 11: selected; not yet completed.
