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

The learner has been away from school for about eight years and is now studying Second Year Mathematics without having taken First Year. Assume that most fundamentals, terminology, givens, question interpretation, theorems, and methods need rebuilding. Explain primarily in Burmese, from first principles: define terms and symbols, identify givens and unknowns, translate the question into a plan, explain why each theorem or method applies, show every calculation step, and point out common mistakes. For English, before starting practice questions from any exam section, first teach that whole section carefully: its purpose, terminology, question patterns, required foundations, rules, recognition clues, step-by-step answering method, model examples, and common mistakes. Check the learner's understanding of this section introduction before beginning its exercises. For sequential English Grammar Pattern study, follow the confirmed workflow in `study-notes/english-learning-plan.md`. Check understanding after each question. Never mark a question complete until the learner explicitly confirms understanding.

## Study Progress

This section is the study-status dashboard. A question is marked **completed** only after it has been explained and the learner has explicitly confirmed understanding. Update the status immediately after that confirmation.

### တွဲဘာသာ Paper Mapping

စာမေးပွဲ paper များကို ၆ ကွာသော တွဲဘာသာများအဖြစ် မှတ်ယူရန် —

- **Paper 2101 ↔ Paper 2107**
- **Paper 2102 ↔ Paper 2108**
- **Paper 2103 ↔ Paper 2109**
- **Paper 2104 ↔ Paper 2110**
- **Paper 2105 ↔ Paper 2111**

Paper တစ်ခု၏ လေ့လာမှုအစီအစဉ်၊ အောင်မှတ်အတွက် ရွေးချယ်မှုနှင့် အချိန်ခွဲဝေမှုများကို ၎င်း၏ တွဲဖက် paper နှင့် ဆက်စပ်စဉ်းစားရန်။

### အမြန်ကြည့်ရန် (လက်ရှိအခြေအနေ)

| အခြေအနေ                                   | အကြောင်းအရာ                                                                                                                                     |
| ------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔁 အရင်ပြန်လေ့လာရန်              | မရှိသေးပါ                                                                                                                                                 |
| ▶️ ဆက်လေ့လာရန်                      | Paper 2109 — harmonic-function problem, closed-circuit problem, gradient problem (နောက်မှပြန်လေ့လာရန်); Paper 2104 — recurrence problem B, C |
| ▶️ နောက်ထပ်လေ့ကျင့်ရန်      | English — Section III, Exercise I No. 2 မှစ၍ source exercises |
| ✅ ပြီးဆုံးပြီးသား                | Paper 2101 No. 5(i), Paper 2102 Unit I No. 4, No. 6, No. 8, No. 9၊ Assignment 1 No. 1, No. 4၊ Assignment 2 No. 4 (Unit II No. 2 နှင့်တူ) နှင့် Unit II No. 2, 5, 6, 7, Paper 2103 Unit 1, English Reading Section I, English Section III foundation/No. 1, English Grammar Patterns 1–20 နှင့် Pattern 14/15/16/17/18/19/20 လေ့ကျင့်ခန်းများ, English PDF Section 13 — To + V1, English PDF Section 15 — Without + V-ing, English PDF Section 16 — By + V-ing, English PDF Section 17 — Either…or / Neither…nor, English PDF Sections 1–10 review exercise (20 questions), English Grammar “It is/It was” exercise 3–6, English Grammar “Omitting Relative Pronouns” PDF exercises 1–4 and practice 1–10, Paper 2109 ရှိ အတည်ပြုပြီးသောမေးခွန်းများ; Paper 2110 Question 1(i)–(v) |
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

#### Paper 2110 — Question 1(i)

- Graph theory အခြေခံစကားလုံးများ — vertex, edge, degree, cycle, connected graph, tree, terminal vertex — ကို ရှင်းပြပြီးနောက် “Tree; all vertices of degree 2” သည် မဖြစ်နိုင်ကြောင်း ရှင်းပြခဲ့သည်။
- Learner က degree, cycle မရှိခြင်းနှင့် terminal vertices ကို နားလည်ကြောင်း အတည်ပြုခဲ့သည်။

#### Paper 2110 — Question 1(ii)

- `E` နှင့် `F` တို့၏ degree သည် `3` ဖြစ်ပြီး `A,B,C,D` တို့၏ degree သည် `1` ဖြစ်ကြောင်း learner က အတည်ပြုခဲ့သည်။
- အဆိုပါ graph သည် connected ဖြစ်ပြီး cycle မရှိသောကြောင့် tree ဖြစ်ကြောင်း ရှင်းပြပြီးသည်။

#### Paper 2110 — Question 1(iii)

- `A—B—C—D—E—F—G` နှင့် isolated vertex `H` ကို အသုံးပြု၍ vertices `8` ခုနှင့် edges `6` ကြောင်းရှိသော graph ကို တည်ဆောက်ပြခဲ့သည်။
- မေးခွန်းတွင် tree သို့မဟုတ် connected ဖြစ်ရမည်ဟု မသတ်မှတ်ထားသောကြောင့် `H` သီးခြားဖြစ်နေလည်း အဖြေမှန်ကြောင်း learner က နားလည်ကြောင်း အတည်ပြုခဲ့သည်။

#### Paper 2110 — Question 1(iv)

- `A—B—C—D—E` နှင့် isolated vertex `F` ကို အသုံးပြု၍ vertices `6` ခု၊ edges `4` ကြောင်းနှင့် cycle မရှိသော graph ကို တည်ဆောက်ပြခဲ့သည်။
- Learner က acyclic ဖြစ်/မဖြစ်သည်မှာ isolated vertex ရှိ/မရှိမဟုတ်ဘဲ loop/cycle ရှိ/မရှိပေါ် မူတည်ကြောင်း အတည်ပြုခဲ့သည်။

#### Paper 2110 — Question 1(v)

- `v1,v2,v3,v4` သည် internal vertices `4` ခု၊ `v5` မှ `v10` သည် terminal vertices `6` ခုဖြစ်ကြောင်း learner က အတည်ပြုခဲ့သည်။
- Graph သည် connected ဖြစ်ပြီး cycle မရှိသောကြောင့် tree ဖြစ်ကြောင်း ရှင်းပြပြီးသည်။

#### Paper 2103 — Unit 1

- No. 5, No. 6, No. 7, No. 10, No. 11 — learner confirmation ရပြီး ပြီးဆုံး။

#### Paper 2101 — No. 5(i)

- `f(z)=iz+2` ကို `z=x+iy` အစားထိုး၍ `f(z)=(2-y)+ix` ဖြစ်ကြောင်းရှင်းပြပြီး `u(x,y)=2-y`, `v(x,y)=x` ဟု ခွဲခြားခဲ့သည်။
- `u_x=0`, `u_y=-1`, `v_x=1`, `v_y=0` ကိုရှာပြီး Cauchy–Riemann equations `u_x=v_y` နှင့် `u_y=-v_x` မှန်ကြောင်း စစ်ဆေးခဲ့သည်။
- `f'(z)=u_x+iv_x=i` နှင့် `f''(z)=0` ကို ရှင်းပြပြီး learner က နားလည်ကြောင်း အတည်ပြုခဲ့သည်။

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

#### English — Grammar: “It is / It was” exercise 3–6

- Cleft sentence ပုံစံဖြင့် အလေးပေးရမည့် အပိုင်းကို ရှေ့တင်ခြင်းကို လေ့ကျင့်ခဲ့သည်။
- No. 3 နှင့် No. 6 ကို မှန်ကန်စွာရေးခဲ့သည်။ No. 4 ၏ရေးပုံကို လက်ခံနိုင်ပြီး underline လုပ်ထားသော prepositional phrase တစ်ခုလုံးကို ရှေ့တင်သည့် စာမေးပွဲအတွက် ပိုသင့်သောပုံစံကိုလည်း ပြန်လည်ရှင်းပြခဲ့သည်။ No. 5 တွင် မူရင်း `students` ကို plural ထားရမည်ကို ပြင်ဆင်ခဲ့သည်။
- Learner က ရှင်းလင်းချက်ကို နားလည်ကြောင်း 2026-09-28 တွင် အတည်ပြုခဲ့သည်။

#### English — Grammar: Omitting Relative Pronouns

- PDF page 4 မှ R.P. (`who`, `whom`, `which`, `that`) ကို object ဖြစ်လျှင် တစ်လုံးတည်းချန်ခြင်း၊ subject ဖြစ်လျှင် `V-ing`/`V3` ဖြင့် relative clause ကို အတိုချုံးခြင်းတို့ကို ရှင်းပြခဲ့သည်။
- PDF exercises 1–4 နှင့် လေ့ကျင့်ခန်းအသစ် 1–10 ကို ဖြေရှင်းခဲ့သည်။ Learner ၏ grammar အဖြေများအားလုံးမှန်ပြီး စာလုံးရိုက်မှားမှု ၂ ခုသာ ပြင်ဆင်ခဲ့သည်။
- Learner က `R.P. + subject + verb` တွင် R.P. ကိုဖြုတ်ပြီး ကျန်တာထားရန်နှင့် `R.P. + be + V-ing` တွင် `R.P. + be` ကိုဖြုတ်ပြီး `V-ing` ကိုထားရန် နားလည်ကြောင်း 2026-09-28 တွင် အတည်ပြုခဲ့သည်။

#### English — Grammar Patterns 1–20

- `english-grammar-short-notes.md` နှင့် `english-grammar-patterns.md` ထဲရှိ numbering အတိုင်း Pattern 1 မှ Pattern 20 အထိ လေ့လာပြီး သင်ခန်းစာများပြီးဆုံးခဲ့သည်။
- Pattern 9–13 သည် `To + V1`, `V-ing`, `Without + V-ing`, `By + V-ing`, `Either ... or / Neither ... nor` ဖြစ်သည်။
- Pattern 14 (`Not only ... but also`) တွင် A/B grammatical form တူညီမှု၊ sentence-initial `Not only` ၌ ပထမ clause သာ inversion ဖြစ်ပုံနှင့် subject–verb agreement ကို ရှင်းပြပြီး learner က 2026-09-29 တွင် နားလည်ကြောင်း အတည်ပြုခဲ့သည်။
- Pattern 14 လေ့ကျင့်ခန်း ၅ ပုဒ်ကို learner က ပြင်ဆင်ချက်များ နားလည်ကြောင်း 2026-09-29 တွင် အတည်ပြုပြီးနောက် ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်ခဲ့သည်။
- Pattern 15 (`so ... that`) ၏ adjective/adverb၊ `so many/few + plural count noun` နှင့် `so much/little + uncountable noun` ပုံစံများကို ရှင်းပြခဲ့သည်။ Learner က မေးခွန်း ၁၀ ပုဒ်ကို ဖြေပြီး ပြင်ဆင်ချက်များကို 2026-09-29 တွင် နားလည်ကြောင်း အတည်ပြုခဲ့သည်။ Pattern 15 ပြီးဆုံးပြီး နောက်တစ်ခုမှာ Pattern 16 ဖြစ်သည်။
- Pattern 16 (`be about to`) တွင် Present/Past/Future active ပုံစံများ၊ passive ပုံစံများနှင့် PDF ၏ Future formula `will be about to + V1` ကို ရှင်းပြခဲ့သည်။ Learner က မေးခွန်း ၅ ပုဒ်လုံးကို မှန်ကန်စွာဖြေပြီး နားလည်ကြောင်း 2026-09-29 တွင် အတည်ပြုခဲ့သည်။ Pattern 16 ပြီးဆုံးပြီး နောက်တစ်ခုမှာ Pattern 17 ဖြစ်သည်။
- Pattern 17 (`have to`) တွင် `have/has/had/will have to + V1`၊ `don't/doesn't have to` နှင့် `mustn't` တို့၏ အဓိပ္ပာယ်ကွာခြားမှုကို ရှင်းပြခဲ့သည်။ Learner က မေးခွန်း ၅ ပုဒ်ကို ဖြေပြီး ပြင်ဆင်ချက်များကို 2026-09-29 တွင် နားလည်ကြောင်း အတည်ပြုခဲ့သည်။ Pattern 17 ပြီးဆုံးပြီး နောက်တစ်ခုမှာ Pattern 18 ဖြစ်သည်။
- Pattern 18 (`by means of`) တွင် `by means of + noun` နှင့် `X enables Y to ...` ကို `By means of X, Y can ...` သို့ ပြောင်းရေးနည်းကို ရှင်းပြခဲ့သည်။ Learner က မေးခွန်း ၅ ပုဒ်ကို ဖြေပြီး ပြင်ဆင်ချက်များကို 2026-09-29 တွင် နားလည်ကြောင်း အတည်ပြုခဲ့သည်။ Pattern 18 ပြီးဆုံးပြီး နောက်တစ်ခုမှာ Pattern 19 ဖြစ်သည်။
- Pattern 19 (`differ in ... from`) တွင် singular/plural subject agreement၊ `in` နောက်က ကွာခြားချက်နှင့် `from` နောက်က နှိုင်းယှဉ်စရာကို ရှင်းပြခဲ့သည်။ Source PDF ၏ slash format (`subject / aspect / comparison`) ဖြင့် မေးခွန်း ၅ ပုဒ်ကို ဖြေပြီး learner က 2026-09-29 တွင် နားလည်ကြောင်း အတည်ပြုခဲ့သည်။ Pattern 19 ပြီးဆုံးပြီး နောက်တစ်ခုမှာ Pattern 20 ဖြစ်သည်။
- Pattern 20 (`as if`) တွင် present unreal `as if + S + V2`၊ past unreal `as if + S + had + V3` နှင့် unreal `be` အတွက် `were` ကို ရှင်းပြခဲ့သည်။ Source slash format ဖြင့် မေးခွန်း ၅ ပုဒ်ကို ဖြေပြီး learner က 2026-09-29 တွင် နားလည်ကြောင်း အတည်ပြုခဲ့သည်။ Grammar Patterns 1–20 ပြီးဆုံးပြီး English grammar pattern sequence တွင် နောက်ထပ် pattern မကျန်ပါ။

#### Paper 2109 — အတည်ပြုပြီးသော မေးခွန်းများ

- **Ex. 1.1** — ထပ်မံ full-mark proof ဖြင့် review ပြီး။
- **MQ No. 2 (Model Question)** — full-mark vector နှင့် scalar-product justification ဖြင့် review ပြီး။
- **S.A. 1.1 (1)** — full-mark theorem wording ဖြင့် review ပြီး။
- **S.A. 1.1 (2)(i) နှင့် (ii)** — တစ်ပုဒ်အဖြစ်တွက်ပြီး determinant signs နှင့် full-mark vector-product working ကို review ပြီး။
- **Ex. 1.2** — full-mark determinant working ဖြင့် review ပြီး။
- **Cross-product foundation review** — right-handed unit-vector rules, reversed-order signs, anti-commutative property, နှင့် vector × itself = zero vector။
- **No. 3** — directional derivative; gradient, unit direction vector, နှင့် dot product ကို အသုံးပြု၍ ဖြေရှင်းပြီး learner confirmation ရရှိ။

#### Paper 2104 — Recurrence Relations: Compound Interest

- **Problem A** — 2000 K ကို 14% annually compounded interest ဖြင့် ရင်းနှီးမြှုပ်နှံသည့် မေးခွန်းကို recurrence relation, initial condition, first terms, explicit formula နှင့် doubling time အပါအဝင် ရှင်းပြပြီး learner က နားလည်ကြောင်း အတည်ပြုခဲ့သည်။

#### Paper 2102 — Unit II No. 2

- `y''+y=0` ကို power-series method ဖြင့် ဖြေရှင်းခဲ့သည်။
- `y=Σ_{n=0}^{∞}c_nx^n` ဟုယူ၍ identity principle အသုံးပြုကာ
  `c_{n+2}=-c_n/[(n+2)(n+1)]` ကိုရရှိခဲ့သည်။
- Even-power နှင့် odd-power series များကို `cos x` နှင့် `sin x` အဖြစ် ခွဲခြားပြီး `y=c_0 cos x+c_1 sin x` ဟုရရှိခဲ့သည်။
- Learner က နားလည်ကြောင်း အတည်ပြုပြီး ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်သည်။

#### Paper 2102 — Unit II No. 5

- `(x-3)y'+2y=0` ကို power-series method ဖြင့် ဖြေရှင်းခဲ့သည်။
- Recurrence relation `c_{n+1}=(n+2)c_n/[3(n+1)]`၊ coefficient formula `c_n=(n+1)c_0/3^n` နှင့် radius of convergence `ρ=3` ကို ရရှိခဲ့သည်။
- Learner က နားလည်ကြောင်း အတည်ပြုပြီး ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်သည်။

#### Paper 2102 — Unit II No. 6

- `(x-1)y'+2y=0` ကို power-series method ဖြင့် ဖြေရှင်းခဲ့သည်။
- Recurrence relation `c_{n+1}=(n+2)c_n/(n+1)`၊ coefficient formula `c_n=(n+1)c_0` နှင့် radius of convergence `ρ=1` ကို ရရှိခဲ့သည်။
- Learner က နားလည်ကြောင်း အတည်ပြုပြီး ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်သည်။

#### Paper 2102 — Unit II No. 7

- `(x^2+1)y''+2xy'-2y=0`၊ `y(0)=0` နှင့် `y'(0)=1` ကို power-series method ဖြင့် ဖြေရှင်းခဲ့သည်။
- Recurrence relation `c_{n+2}=(1-n)c_n/(n+1)` မှတစ်ဆင့် `c_0=0`, `c_1=1` နှင့် အခြား coefficients များ သုညဖြစ်ကြောင်း ရှာဖွေခဲ့သည်။
- Required solution သည် `y=x` ဖြစ်ကြောင်း အတည်ပြုခဲ့သည်။ PDF ထဲက `y'(0)=1 ⇒ c_1=0` သည် typo ဖြစ်ပြီး `c_1=1` ဖြစ်ရမည်။
- Learner က နားလည်ကြောင်း အတည်ပြုပြီး ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်သည်။

#### Paper 2102 — Unit I No. 8

- `y''-2y'+2y=x+1`၊ `y(0)=3` နှင့် `y'(0)=0` ကို characteristic-equation method ဖြင့် ဖြေရှင်းခဲ့သည်။
- Complementary solution `y_c=e^x(C_1 cos x+C_2 sin x)`၊ particular solution `y_p=(1/2)x+1` နှင့် initial conditions မှ `C_1=2`, `C_2=-5/2` ကို ရရှိခဲ့သည်။
- Final solution `y=e^x(2 cos x-(5/2) sin x)+(1/2)x+1` ဖြစ်ကြောင်း learner က နားလည်ကြောင်း အတည်ပြုပြီး ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်သည်။

#### Paper 2102 — Unit I No. 6

- `y''+6y'+13y=e^{-3x}\cos 2x` အတွက် complementary solution `y_c=e^{-3x}(C_1\cos 2x+C_2\sin 2x)` ကို ရှာဖွေခဲ့သည်။
- RHS ပုံစံအရ မူလ particular form `e^{-3x}(A\cos 2x+B\sin 2x)` ဖြစ်သော်လည်း `y_c` နှင့် ထပ်နေသောကြောင့် `x` တစ်ခါမြှောက်ရပြီး appropriate form သည် `y_p=xe^{-3x}(A\cos 2x+B\sin 2x)` ဖြစ်ကြောင်း ရှင်းပြခဲ့သည်။
- Learner က Unit I No. 6 ကို နားလည်ကြောင်း အတည်ပြုပြီး ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်သည်။

#### Paper 2102 — Unit I No. 4

- ပေးထားသော linearly independent solutions `y_1=e^x`, `y_2=e^{2x}`, `y_3=e^{3x}` ကို အသုံးပြု၍ third-order homogeneous equation ၏ general solution `y=C_1e^x+C_2e^{2x}+C_3e^{3x}` ကို ရေးခဲ့သည်။
- `y(0)=0`, `y'(0)=0`, `y''(0)=3` ကို အသုံးပြု၍ `C_1=3/2`, `C_2=-3`, `C_3=3/2` ရှာဖွေခဲ့သည်။
- Particular solution `y=(3/2)e^x-3e^{2x}+(3/2)e^{3x}` ဖြစ်ကြောင်း learner က နားလည်ကြောင်း အတည်ပြုပြီး ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်သည်။

#### Paper 2102 — Unit I No. 9

- `y''+3y'+2y=4e^x` ကို variation of parameters ဖြင့် ဖြေရှင်းခဲ့သည်။ Homogeneous solutions `y_1=e^{-x}`, `y_2=e^{-2x}` နှင့် Wronskian `W=-e^{-3x}` ကို ရှာဖွေခဲ့သည်။
- `y_p=u_1y_1+u_2y_2` ဟုယူပြီး auxiliary condition `u_1'y_1+u_2'y_2=0` မှတစ်ဆင့် `u_1'=-y_2g/W`, `u_2'=y_1g/W` formula များထွက်လာပုံကို ရှင်းပြခဲ့သည်။
- `u_1=2e^{2x}`, `u_2=-(4/3)e^{3x}` ရရှိပြီး particular solution `y_p=(2/3)e^x` ဖြစ်ကြောင်း learner က နားလည်ကြောင်း အတည်ပြုပြီး ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်သည်။

#### Paper 2102 — Assignments

- **Assignment 1 No. 1** — (i) `y_1=e^x cos x` နှင့် `y_2=e^x sin x` တို့ကို `y''-2y'+2y=0` ထဲ substitute လုပ်၍ solution များဖြစ်ကြောင်း စစ်ဆေးခဲ့သည်။ (ii) `9y''-12y'+4y=0` အတွက် characteristic equation `9r^2-12r+4=(3r-2)^2=0` မှ repeated root `r=2/3` ရပြီး general solution `y=(C_1+C_2x)e^{2x/3}` ရရှိခဲ့သည်။ Learner က နားလည်ကြောင်း အတည်ပြုပြီး ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်သည်။
- **Assignment 1 No. 4** — `y'''+3y''-10y'=0`၊ `y(0)=7`, `y'(0)=0`, `y''(0)=70` ကို characteristic-equation method ဖြင့် ဖြေရှင်းပြီး `y=2e^{-5x}+5e^{2x}` ရရှိခဲ့သည်။
- **Assignment 2 No. 4** — `y''+y=0` ကို power-series method ဖြင့် ဖြေရှင်းသည့် မေးခွန်းဖြစ်ပြီး Unit II No. 2 နှင့် တူညီသောကြောင့် ထို completion နှင့်အတူ covered ဖြစ်သည်။
- Learner က Assignment 1 No. 1 နှင့် No. 4 ကို နားလည်ကြောင်း အတည်ပြုပြီး ပြီးဆုံးအဖြစ် မှတ်တမ်းတင်သည်။

### 📚 ကိုးကားရန်နှင့် နောင်ပြန်ကြည့်ရန်

- **Trigonometric ratios foundation** — SOH-CAH-TOA, special-angle values `0°`, `30°`, `45°`, `60°`, `90°`, horizontal component `F cos θ`, vertical component `F sin θ`။ အသေးစိတ် Burmese notes ကို [`study-notes/trigonometric-ratios.md`](study-notes/trigonometric-ratios.md) တွင် သိမ်းထားသည်။ လိုအပ်သလို ပြန်လေ့လာရန်။
- Paper 2103 Unit 1 ရွေးထားသော မေးခွန်းများ၏ full working ကို [`study-notes/2103-unit-1-selected-solutions.md`](study-notes/2103-unit-1-selected-solutions.md) တွင် သိမ်းထားသည်။
- Paper 2109 Unit 1 ရွေးထားသော မေးခွန်းများ၏ solution notes နှင့် confirmation status ကို [`study-notes/2109-unit-1-selected-solutions.md`](study-notes/2109-unit-1-selected-solutions.md) တွင် သိမ်းထားသည်။
- English learning plan ကို [`study-notes/english-learning-plan.md`](study-notes/english-learning-plan.md) တွင် သိမ်းထားသည်။ Future English notes များကို `study-notes/` အောက်တွင် `english-` prefix ဖြင့် သိမ်းရန်။
- Paper 2103 confirmed reference pages — `study-pages/2103/unit-1/`: `page-02.png` (No. 5), `page-03.png` (No. 6–7), `page-05.png` (No. 10), `page-06.png` (No. 11)။ အခြား renders များကို `tmp/` အောက်တွင်သာထားရန်။
- English confirmed reference pages များကို `study-pages/eng/<unit>/` တွင်ထားရန်။ Temporary renders များကို `tmp/pdfs/eng/` တွင်ထားရန်။
- Paper 2109 ၏ နောက်ထပ် solution များတွင် theorem/identity အမည်များနှင့် mark-scheme-ready working အပြည့်အစုံ ထည့်ရန်။
