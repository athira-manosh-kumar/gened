# GeneEd MVP
A responsive, buildless genetics learning product. Open `dist/index.html` directly or run `python3 -m http.server 4173 --directory dist`, then visit http://localhost:4173.

## Functional
- Student dashboard derived from local activity progress; fictional Alex Lee profile.
- Three-step DNA lesson and complementary base-pair activity.
- Live Punnett squares for pea flower color and seed shape, nine parent combinations each; phenotype and genotype probabilities.
- Four-question quiz, answer explanations, review, retry and badge for 3/4 or better.
- Browser-local persistence and reset; no account or server required.
- Semantic navigation, skip link, keyboard inputs, visible focus, responsive layouts and live feedback.

## Placeholder / future scope
No authentication, cloud database, real students, teacher tools, videos, DNA extraction or PCR labs. Sample profile is synthetic. No user research or measured learning outcomes are claimed. DNA illustration is schematic. Google fonts are optional; system fonts work offline.

## Science
Single-locus, two-allele, complete-dominance models with independent offspring outcomes. Pea purple flower and round seed alleles are dominant in these examples. Dominance is not strength or frequency. Many real traits are polygenic or affected by environment. See in-product About for OpenStax and NHGRI references.

## Validation
Run `node tests/engine.test.cjs` to verify 18 crosses, known probabilities and reciprocal symmetry. Browser QA is documented in QA.md.

## Portfolio framing
Concept MVP, not a launched education business. Proposed design principle: connect explanation → hands-on exploration → corrective feedback. Future research: test vocabulary comprehension, simulator interpretation and independent learning with introductory biology students. These are proposed research activities, not completed research.

## Visual refresh
The updated theme uses cobalt, navy and coral. Local JPEG assets show a realistic DNA molecular illustration and photographic-style pea/lab scenes; they are AI-generated, as documented in ASSETS.md. Original vector logo is embedded as SVG.
