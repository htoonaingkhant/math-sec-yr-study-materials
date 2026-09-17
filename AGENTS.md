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

The learner has been away from school for about eight years and is now studying Second Year Mathematics without having taken First Year. Assume that most fundamentals, terminology, givens, question interpretation, theorems, and methods need rebuilding. Explain primarily in Burmese, from first principles: define terms and symbols, identify givens and unknowns, translate the question into a plan, explain why each theorem or method applies, show every calculation step, and point out common mistakes. For English, before starting practice questions from any exam section, first teach that whole section carefully: its purpose, terminology, question patterns, required foundations, rules, recognition clues, step-by-step answering method, model examples, and common mistakes. Check the learner's understanding of this section introduction before beginning its exercises. Check understanding after each question. Never mark a question complete until the learner explicitly confirms understanding.

## Study Progress

This section is the study-status dashboard. A question is marked **completed** only after it has been explained and the learner has explicitly confirmed understanding. Update the status immediately after that confirmation.

### အမြန်ကြည့်ရန် (လက်ရှိအခြေအနေ)

| အခြေအနေ                                   | အကြောင်းအရာ                                                                                                                                     |
| ------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔁 အရင်ပြန်လေ့လာရန်              | မရှိသေးပါ                                                                                                                                                 |
| ▶️ ဆက်လေ့လာရန်                      | Paper 2109 — harmonic-function problem, closed-circuit problem, gradient problem (နောက်မှပြန်လေ့လာရန်); Paper 2102 — ရွေးချယ်ထားသော Unit I, Unit II နှင့် Assignment မေးခွန်းများ |
| ▶️ နောက်ထပ်လေ့ကျင့်ရန်      | English — Section III, Exercise I No. 2 မှစ၍ source exercises                                                                                         |
| ✅ ပြီးဆုံးပြီးသား                | Paper 2103 Unit 1, English Reading Section I, English Section III foundation/No. 1, Paper 2109 ရှိ အတည်ပြုပြီးသောမေးခွန်းများ |
| 📚 လိုအပ်သလို ပြန်ကြည့်ရန် | Trigonometric-ratios foundation notes                                                                                                                      |

### အခြေအနေအဓိပ္ပါယ်

- ✅ **ပြီးဆုံးပြီးသား** — ရှင်းပြပြီး learner က နားလည်ကြောင်း အတည်ပြုပြီးသား။
- 🔁 **ပြန်လေ့လာရန်** — ရှင်းပြပြီးသားဖြစ်သော်လည်း ပြန်သုံးသပ်ပြီးမှ completion အဖြစ် အတည်ပြုရန်ကျန်။
- ▶️ **ဆက်လေ့လာရန်** — ရွေးထားပြီးသော်လည်း မေးခွန်းအဖြစ် မပြီးဆုံးသေး။
- 📚 **ကိုးကား/ပြန်ကြည့်ရန်** — မေးခွန်းတစ်ပုဒ်၏ completion status မဟုတ်ဘဲ နောင်ပြန်အသုံးပြုရန် note သို့မဟုတ် reference။

### ✅ အခု ပြန်လေ့လာပြီး အတည်ပြုပြီး

#### Paper 2109 — No. 3

- **မေးခွန်းအမျိုးအစား** — Directional derivative.
- **ပေးထားချက်** — `φ = x²yz + 4xz²`, point `(1, -2, -1)`, direction `2i - j - 2k`.
- Gradient, unit direction vector, scalar product အဆင့်များကို ပြန်လည်ရှင်းပြပြီး learner က နားလည်ကြောင်း အတည်ပြုခဲ့သည်။
- အဖြေ — `37/3`။
- အစောပိုင်းတွင် ဖတ်မှားပြီး ဖြေထားသော line-integral response သည် ဤ No. 3 ၏အဖြေမဟုတ်ပါ။

### ▶️ ဆက်လေ့လာရန်ကျန်

#### Paper 2109 — ရွေးထားသော မေးခွန်းများ

အောက်ပါမေးခွန်းများကို **No. 3 ပြန်လေ့လာပြီးနောက်** အစဉ်လိုက် ဆက်ရှင်းပြရန် —

1. **“If `r = [x, y, z]`, prove that …”** — harmonic function problem; explanation deferred for later because it was difficult.
2. **“If `C` is a closed circuit …”** — closed-circuit problem; this is the later No. 2, not MQ No. 2; explanation given but learner confirmation pending; defer for later.
3. **“Find the gradient of the function …”** — gradient problem.

#### Paper 2102 — ရွေးထားသော မေးခွန်းများ

- **Unit I** — No. 4, 6, 8, 9
- **Unit II** — No. 5, 6, 7
- **Assignment 1** — No. 1, 4
- **Assignment 2** — No. 4
- လက်ရှိရရှိထားသော reference images များကို အောက်ပါအတိုင်း သိမ်းထားသည် —
  - `study-pages/2102/assignment-1/2102-assignment-1-no-1.png`
  - `study-pages/2102/assignment-1/2102-assignment-1-no-4-part-1.png`
  - `study-pages/2102/assignment-1/2102-assignment-1-no-4-part-2.png`
  - `study-pages/2102/assignment-2/2102-assignment-2-no-4.png`

#### English — Section IIIm

- Word Forms foundation lesson နှင့် Section III opening review ပြီးဆုံးပြီးဖြစ်သည်။
- Section III, Exercise I **No. 1** ပြီးဆုံးပြီးဖြစ်သည်။
- ထို့ကြောင့် source exercises ကို **Exercise I No. 2 မှစ၍** question by question ဆက်လေ့ကျင့်ရန်။

### ✅ ပြီးဆုံးပြီးသား

#### Paper 2103 — Unit 1

- No. 5, No. 6, No. 7, No. 10, No. 11 — learner confirmation ရပြီး ပြီးဆုံး။

#### English — Reading Section I

- **I(a) Reference words** — “This movement,” “It,” “them,” “These groups,” “which” တို့၏ ရည်ညွှန်းချက်များကို ရှာဖွေခြင်း။
- **I(b) Matching** — paraphrased descriptions နှင့် မှန်ကန်သော people/activities ကို တွဲခြင်း။
- **I(c) True / False** — passage evidence နှင့် “all,” “completely,” “some” ကဲ့သို့ limiting words များကို သတိပြုခြင်း။
- **I(d) Passage questions** — why/how/result မေးခွန်းများကို complete sentences ဖြင့် ဖြေခြင်းနှင့် `could be saved` ကဲ့သို့ passive forms ကို ပြင်ဆင်ခြင်း။
- Reading Section I တစ်ခုလုံး ပြီးဆုံး။

#### English — Section III Word Forms

- Noun, adjective, adverb, verb forms ရွေးချယ်ခြင်း — `refusal`, `improvements`, `useful/used`, `enlarge`။
- Section III opening review အပြည့်အစုံ — learner confirmation ရပြီး ပြီးဆုံး။
- Exercise I No. 1 — `to be + adjective` (`healthy`) နှင့် noun ကို ဖော်ပြသော coordinated adjectives (`nutritious and fresh fruit`)။

#### Paper 2109 — အတည်ပြုပြီးသော မေးခွန်းများ

- **Ex. 1.1** — ထပ်မံ full-mark proof ဖြင့် review ပြီး။
- **MQ No. 2 (Model Question)** — full-mark vector နှင့် scalar-product justification ဖြင့် review ပြီး။
- **S.A. 1.1 (1)** — full-mark theorem wording ဖြင့် review ပြီး။
- **S.A. 1.1 (2)(i) နှင့် (ii)** — တစ်ပုဒ်အဖြစ်တွက်ပြီး determinant signs နှင့် full-mark vector-product working ကို review ပြီး။
- **Ex. 1.2** — full-mark determinant working ဖြင့် review ပြီး။
- **Cross-product foundation review** — right-handed unit-vector rules, reversed-order signs, anti-commutative property, နှင့် vector × itself = zero vector။
- **No. 3** — directional derivative; gradient, unit direction vector, နှင့် dot product ကို အသုံးပြု၍ ဖြေရှင်းပြီး learner confirmation ရရှိ။

### 📚 ကိုးကားရန်နှင့် နောင်ပြန်ကြည့်ရန်

- **Trigonometric ratios foundation** — SOH-CAH-TOA, special-angle values `0°`, `30°`, `45°`, `60°`, `90°`, horizontal component `F cos θ`, vertical component `F sin θ`။ အသေးစိတ် Burmese notes ကို [`study-notes/trigonometric-ratios.md`](study-notes/trigonometric-ratios.md) တွင် သိမ်းထားသည်။ လိုအပ်သလို ပြန်လေ့လာရန်။
- English learning plan ကို [`study-notes/english-learning-plan.md`](study-notes/english-learning-plan.md) တွင် သိမ်းထားသည်။ Future English notes များကို `study-notes/` အောက်တွင် `english-` prefix ဖြင့် သိမ်းရန်။
- Paper 2103 confirmed reference pages — `study-pages/2103/unit-1/`: `page-02.png` (No. 5), `page-03.png` (No. 6–7), `page-05.png` (No. 10), `page-06.png` (No. 11)။ အခြား renders များကို `tmp/` အောက်တွင်သာထားရန်။
- English confirmed reference pages များကို `study-pages/eng/<unit>/` တွင်ထားရန်။ Temporary renders များကို `tmp/pdfs/eng/` တွင်ထားရန်။
- Paper 2109 ၏ နောက်ထပ် solution များတွင် theorem/identity အမည်များနှင့် mark-scheme-ready working အပြည့်အစုံ ထည့်ရန်။
