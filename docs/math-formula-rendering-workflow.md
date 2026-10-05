# Math Formula Rendering Workflow

This is the reusable workflow for every study artifact that contains mathematical formulas: formula sheets, selected-question summaries, solution notes, image exports, and phone-readable PDFs. It applies to every paper and subject, not only Paper 2109.

## Goal

Produce one readable artifact in which:

- ordinary Burmese prose is Unicode text;
- ordinary prose uses a Myanmar-capable font, preferably Noto Sans Myanmar;
- English headings may use a separate readable sans-serif font;
- mathematical notation is rendered as an equation, not assembled from manually positioned characters;
- the source/teacher's vector notation is preserved exactly—if vectors are shown with an underline below the character, keep the underline below the character rather than converting it to an arrow;
- vector marks, unit-vector hats, square roots, fractions, determinants, gradients, integrals, subscripts, superscripts, and parentheses stay attached to the correct symbols;
- several pages are delivered as one PDF for easier phone viewing;
- the original scanned PDF/image is never overwritten.

## Why the previous approach failed

Manually placing Unicode arrows, underlines, hats, radicals, and mathematical glyphs with ordinary text fonts caused symbols to drift above or below the intended character. A Myanmar font also should not be used as the math font. Font substitution can make the result look different on another phone.

The reliable approach is to keep the two text systems separate:

1. Render Burmese and normal explanatory text with a Myanmar-capable Unicode font.
2. Render every formula with MathJax (TeX input to SVG/PNG), so the complete equation—including accents, arrows, radicals, fractions, and spacing—is laid out by the equation renderer.
3. Place the resulting equation image onto the page as one object.

Cambria Math does not need to be installed for this workflow. The formula is rendered before the PDF is assembled, so the final appearance does not depend on whether the phone has Cambria Math installed.

## Repeatable steps

### 1. Read the source and preserve it

Read the repository `AGENTS.md` first. Identify the selected questions in source/PDF order and verify the question numbers against the scan or confirmed reference images. Keep the source scan unchanged.

Use a derived filename that keeps the paper identifier, for example:

```text
output/pdf/2109-formula-and-question-map.pdf
```

For another paper, replace `2109` with that paper's identifier and use a descriptive suffix.

### 2. Prepare the content

Write ordinary explanations as Unicode Burmese. Do not type Burmese in Zawgyi encoding. Keep formula content in TeX strings rather than plain text.

Use TeX constructs for the notation that previously drifted, and preserve the notation used by the teacher/source. For example, if the teacher uses an underline below vector characters, use `\underline{a}` (or the equivalent supported by the renderer) for vectors rather than changing them to `\vec a` or `\overrightarrow{a}`:

```tex
\underline{a},\quad \underline{b},\quad \hat{\mathbf{i}},\quad
\sqrt{a_1^2+a_2^2+a_3^2},\quad
\frac{\underline{d}}{|\underline{d}|},\quad
\begin{vmatrix}a_1&a_2&a_3\\b_1&b_2&b_3\\c_1&c_2&c_3\end{vmatrix}
```

Use a question-number-to-formula map when the learner asks for fast memorisation. Keep the source question order and label each item clearly.

### 3. Render formulas separately

Use MathJax through the bundled Node runtime. The working implementation used `mathjax-full` and converted the resulting SVG equations to transparent PNGs before placing them on the page.

Keep the renderer's formula font independent from the Burmese prose font. Do not manually position a separate underline, arrow, or hat over a letter. Do not replace rendered formulas with a string such as `sqrt(...)` when the learner requested exact notation. The teacher/source notation has priority: underline stays underline, arrow stays arrow, and a unit-vector hat stays a hat.

If the runtime package is not already available, install it locally under the paper's temporary build directory, not globally and not into the source-document area. Store intermediate renders under `tmp/pdfs/<paper>/`.

### 4. Compose pages

Use a phone-readable page size and generous spacing. A4 pages at approximately 1240 × 1754 pixels worked well for the formula sheet. Use separate styling for:

- Burmese prose: a Myanmar Unicode font such as Noto Sans Myanmar;
- English headings: a readable sans-serif font;
- formulas: MathJax-rendered equation images.

If the result would be two or more images, combine all pages into one PDF. Keep the formula map and the last-minute memory chain in the same PDF when requested.

### 5. Verify before delivery

Always perform the render-and-inspect loop:

1. Run `pdfinfo` and confirm the expected page count, page size, and no encryption.
2. Run `file` on the output PDF.
3. Render the final PDF back to page images with Poppler `pdftoppm`.
4. Visually inspect every rendered page, not only the first page.
5. Check that Burmese characters are readable Unicode text, formulas are not clipped, and the source notation (including underlines below vector characters, arrows, hats, subscripts, superscripts, fractions, determinants, and integrals) remains correctly attached.
6. Check the bottom margin and footer for overlap or truncation.
7. Confirm the original scan is unchanged and temporary renders remain under `tmp/pdfs/<paper>/`.

Completion means all pages pass the visual check and `pdfinfo` reports the expected count. Do not deliver an uninspected PDF.

## Reference implementation from the first successful run

The first successful run for Paper 2109 used:

- a Node script under `tmp/pdfs/2109/create_formula_mathjax.js`;
- MathJax TeX → SVG → PNG for formulas;
- Noto Sans Myanmar for ordinary Burmese text;
- Pillow to combine four page PNGs into `output/pdf/2109-formula-and-question-map.pdf`;
- bundled `pdfinfo`, `pdftoppm`, and visual inspection of all four final pages.

The Paper 2109 filenames are examples only. Apply the same separation of prose and math, the same single-PDF preference, and the same complete QA loop to every future math-formula artifact.
