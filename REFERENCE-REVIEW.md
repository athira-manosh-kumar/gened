# GeneEd reference review and product direction
Reviewed 12 October 2026. This is reference research and design synthesis, not completed learner research or evidence of learning effectiveness.

## Main conclusion
The core should be a manipulable science workbench. Each learner action must change a modeled state, produce inspectable evidence, or influence an interpretation. The learner should be able to undo, compare and retry. Explanations should help interpret an observation at the point of need.

Learn, practise and experiment should be three ways to use the same scientific model:
- Guided discovery: hints, labeled equipment/data and explanations.
- Free exploration: editable inputs, immediate outputs, comparison and reset.
- Challenge: an investigation goal, less guidance and feedback on reasoning.

Different levels should change the amount of scaffolding and complexity, rather than simply change page copy.

## References and implications

### 1. University of Utah Learn.Genetics — Mutate a Gene
https://learn.genetics.utah.edu/content/genetics/mutate/
The resource describes changing DNA and inspecting resulting mRNA/protein changes. It explains codons, reading frames, substitutions and insertion/deletion effects.
Design implication: a learner should directly edit a toy coding sequence and compare codon/amino-acid outputs. Include silent, missense, premature-stop, frameshift and in-frame examples. A change in a translated sequence is not automatically a demonstrated functional or health effect.
Verification: page text was inspected in the browser; the embedded interactive did not fully render, so its editing behavior was not tested firsthand.

### 2. HHMI BioInteractive — Bacterial Identification Virtual Lab
https://www.biointeractive.org/classroom-resources/bacterial-identification-virtual-lab
Its official description connects virtual sample preparation, PCR, electrophoresis, sequencing and analysis to identifying bacteria using 16S sequence information.
Design implication: use an unknown-sample question to connect techniques, rather than presenting disconnected equipment tutorials. Each step should answer why the technique is useful.
Verification: official resource description and learning targets reviewed; the full interactive was not completed.

### 3. LabXchange — Simulations as a Teaching Tool
https://help.labxchange.org/en/articles/7241089
LabXchange describes outcomes that depend on learner actions, and guidance levels that alter prompts while preserving the underlying experimental process.
Design implication: beginners and confident learners can share one workbench. Guided mode explains decisions; challenge mode reduces hints. Avoid an empty expertise selector that only changes wording.

### 4. LabXchange — Simulations
https://help.labxchange.org/en/articles/7239233
The official description includes virtual notebooks, restarting steps, trying different inputs and comparing predictions with outcomes.
Design implication: include an experiment notebook, prediction field, run history and a comparison between runs. A failed attempt should remain useful evidence, not only receive a red error state.

### 5. Cold Spring Harbor Laboratory — DNA Subway 2.0
https://www.cshl.edu/cshl-launches-dna-subway-2-0/
https://dnalc.cshl.edu/assets/files/dnalc-live/Using-DNA-Subway-to-Analyze-Sequence-Barcodes-05182018-Student.pdf
The official descriptions connect education with sequence-analysis workflows. The teaching guide discusses imperfect sequence data, quality inspection and consensus building.
Design implication: sequencing should not be an instant perfect string. Show uncertain calls, compare supporting reads and let the learner distinguish an error from a supported difference. Start with short, synthetic examples.
Verification: descriptions and teaching guide reviewed; DNA Subway itself was not operated.

### 6. Eterna
https://eternagame.org/
https://eternagame.org/edu
Eterna uses RNA-design puzzles and connects selected player designs to experimental testing by researchers.
Design implication: give learners a concrete design goal, allow repeated attempts, and expose the feedback behind the score. GeneEd should not imply its toy models produce experimentally validated molecules or research contributions.
Verification: official product and education descriptions reviewed; gameplay was not tested.

### 7. HHMI BioInteractive — Winogradsky Column
https://www.biointeractive.org/classroom-resources/winogradsky-column-microbial-ecology-bottle
The resource uses a virtual column to explore microbial diversity, metabolic strategies and environmental gradients.
Design implication: microbiology can teach relationships and environments, not only names or harmful microbes. A future simplified community model could let learners change conditions and compare ecological outcomes, with its assumptions stated.
Verification: official resource reviewed; the embedded simulation was blocked in the browser, so its controls were not tested.

### 8. Genomics England — Understanding genomics
https://www.genomicsengland.co.uk/genomic-medicine/understanding-genomics?chapter=panel-bioinformatics
The resource separates sequencing, reads, reference sequences, mapping, variants and bioinformatics.
Design implication: keep generation of sequence evidence distinct from interpretation. The learner should understand how the evidence was produced before receiving a variant label.

### 9. Google DeepMind — AlphaMissense
https://deepmind.google/blog/a-catalogue-of-genetic-mutations-to-help-pinpoint-the-cause-of-diseases/
https://deepmind.google/research/publications/21083/
The primary descriptions concern predictions about missense variants and explicitly require other evidence for interpretation; the model does not directly predict mutation-induced structural changes.
Design implication: a future AI investigation should teach prediction versus evidence. Do not animate a supposedly exact protein shape or equate a score with a diagnosis. Any educational ranking must be labeled simulated unless a real integration exists.

### 10. Google DeepMind — AlphaGenome
https://deepmind.google/blog/alphagenome-ai-for-better-understanding-the-genome/
This reference extends variant-effect predictions into processes such as expression and splicing.
Design implication: later modules should show that sequence changes can affect regulation and RNA processing as well as protein-coding sequence. This is later scope, not justification for a fake biological prediction engine.

## What is missing in the current MVP
- The sequence activity identifies one prepared difference; it does not yet simulate reads, quality or assembly.
- The inheritance investigation reveals a prepared cross; free parent selection exists separately.
- The growth model offers limited controls and an abrupt artificial cap.
- There is no shared workbench, run comparison or experiment notebook.
- “More depth” expands notes but does not yet provide harder experimental decisions.

The current tools are foundation activities. They are not yet the full playable-lab experience requested by the user.

## Recommended next build

### A. Mutation workbench
Editable synthetic coding-strand DNA → corresponding RNA → codons → amino-acid sequence.
Actions: substitute, insert, delete, undo and reset.
Outputs: aligned before/after sequences, codon regrouping, translated amino acids and explicit model limits.
Challenges: change DNA without changing an amino acid; introduce an earlier stop; compare one-base and three-base deletions.
Use a specified reading frame and standard-code toy model. Do not infer disease or exact protein shape from an edit.

### B. Sequencing detective
Synthetic sample → short overlapping reads → inspect uncertainty → align/assemble → compare with a reference → justify a conclusion.
Actions: inspect a read, retain/discard uncertain evidence, place fragments, request another supporting read and compare candidates.
Challenges: distinguish a low-quality miscall from a supported substitution; resolve a sequence with insufficient evidence; identify an unknown microbial sample from a small curated synthetic dataset.
Do not represent a tiny educational match as validated species identification.

### C. Microbial ecosystem
A clearly simplified model of environmental preferences and population interactions.
Actions: change an environmental condition, advance model time and compare runs.
Outputs: population/gradient changes and model assumptions.
This extends microbiology beyond the current generic doubling model.

## Acceptance criteria for an authentic learning interaction
1. Inputs are meaningfully editable.
2. Outputs follow a documented rule or stated model, not an unrelated animation.
3. Different valid inputs can produce different outcomes.
4. Learners can inspect evidence, uncertainty and assumptions.
5. Reset, undo or rerun makes experimentation easy.
6. Feedback explains a mechanism and invites a next experiment.
7. Guided mode and challenge mode use the same underlying model.
8. A final unfamiliar task checks transfer, not recognition of the answer just shown.

## Research still needed
Observe curious beginners and biology learners completing a new investigation. Test whether they can explain the mechanism and uncertainty afterward. Reference products inform design decisions; they do not prove GeneEd's effectiveness or validate all audience needs.
