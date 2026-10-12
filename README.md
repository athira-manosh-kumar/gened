# GeneEd · Genomics and microbiology learning MVP

GeneEd helps curious people build understanding through three pathways: Learn, Practise and Virtual experiments. It welcomes beginners and offers optional deeper notes for familiar learners. Current content covers foundations; it is not a comprehensive specialist course.

## Run locally
Open `dist/index.html` directly, or run `python3 -m http.server 4189 --directory dist` and visit http://localhost:4189. No build step, account or dependencies required. Google fonts are optional; local system fonts work offline.

## Working product
- Discovery hub with three exploration modes, starting-point preference and a next activity based on local progress.
- Topic library connecting genetics, genomics and microbiology.
- Existing three-step DNA lesson, base-pair activity, two-trait Mendelian cross simulator and four-question genetics check.
- Genomics lesson: distinguish gene and genome, find a synthetic sequence substitution, explain why an observed difference does not establish an effect.
- Microbiology lesson: interactive comparison of bacteria, viruses and microscopic fungi, plus an applied yeast question.
- Guided inheritance investigation: hypothesize, examine a cross and explain a recessive phenotype.
- Growth investigation: predict population across generations, compare an unlimited model with an explicitly artificial resource cap, explain limits.
- Six-question mixed challenge with answer reasoning and review links based on missed concepts.
- Searchable glossary, expanded notes, responsive layouts, native labeled inputs, live feedback, semantic SVG icons and keyboard-operable pathway tabs.
- Four locally recorded investigations. Preferences and completion persist in this browser. Quiz state within an attempt is session-only; best mixed score is local.

## Scope and honest limitations
Explorer is a synthetic learner identity. All sequences and growth populations are teaching data. The growth model is mathematical, not a species-specific experimental simulation. No authentication, cloud sync, real learner analytics, physical-lab skills validation or exam-board alignment. PCR, DNA extraction and advanced specialist courses are future scope.

## Scientific basis
See in-product About for NHGRI, OpenStax and Microbiology Society links. Images are generated editorial visuals; ASSETS.md documents provenance. DNA artwork is not a scale model or microscopy.

## Project files
- dist/index.html: shell and editable DNA logo
- dist/style.css: responsive visual system
- dist/app.js: original genetics tools and route integration
- dist/learning.js: new learning pathways and investigations
- dist/engine.js: Mendelian cross arithmetic
- tests/engine.test.cjs: 18 crosses, reciprocal symmetry and known probabilities
- QA.md: observed verification and limits
- PRODUCT-BRIEF.md: product purpose, hypotheses and proposed research

Run `node tests/engine.test.cjs` for genetics calculation checks.
