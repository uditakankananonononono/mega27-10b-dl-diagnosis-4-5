# MEGA27-10b - Diagnoses 4-5 (malaria, pneumonia) - COMPLETION PREREG v2 (locked 2026-09-26 16:24 IST)
Reality (post-clone audit): 10.4 malaria + 10.5 pneumonia ALREADY BUILT in mega27-10-dl-diagnosis-suite/
subitems_4_5 (CNN+RegionGCN, confident-learning census, papers 56/57pp, judge loops 6 and 2 rounds).
Lane-closed 13:03 IST as AI-judged after she DECLINED blinded human expert review (her verbatim 13:03:40: 'Don't email, just put anything. No. For second question'); the closure act itself was the lane's, and it predates + does not exempt these projects from the 4:11 rules. mega27-10b repo = empty; this lane
migrates the projects here as standalone + upgrades both to the 4:11 standard.
Rules: 4:11:18 (10+ judge rounds, negatives never terminal), 4:11:49 (beat benchmarks + NEW DISCOVERY each),
4:12:25 (ChatGPT redirection when stuck), 4:14:37 (ISEF-winner archetype), 13:09:44 (paper PDF attached to
every ChatGPT weakness round). Verified verbatim in phone_messages.

## GATE M4 (malaria benchmark BEAT): named published comparator on identical official test set (n=2758).
Comparators: Rajaraman et al. 2018 (dataset authors) published per-model accuracies (custom CNN 95.9%,
pretrained ResNet-50 headline) - exact target numbers locked from the paper's tables at write-up time.
Current: CNN 0.9608 / AUC 0.9929, cluster-bootstrap CI [95.22,96.89]. Beat = lower CI bound above the
published number, patient/smear-cluster bootstrap preserved.

## GATE M5 (malaria DISCOVERY): confident-learning label-noise census with content-hashed flagged IDs +
measured retraining deltas - framed as first public label-error census of the NIH malaria release.
Verify novelty claim against the 197-PMID lit audit before asserting.

## GATE P4 (pneumonia benchmark BEAT): Kermany et al. 2018 published 92.8% accuracy on the official
624-image test set (verified via PMC10660141). CURRENT STATE DOES NOT BEAT: best committed test acc 0.8413
(gcn_tuned); threshold tuning on OOF gives nothing (OOF-optimal t=0.48 ~= 0.5; train->test shift is the
real gap); torchxrayvision zero-shot 0.38 (documented negative).
LOCKED IMPROVEMENT LADDER (stop at first honest beat):
 L1 frozen ImageNet features (resnet18, single extraction pass) + trained head, threshold frozen from
    OOF only, ONE test evaluation after freeze.
 L2 full fine-tune (10-15 epochs, checkpointed) if L1 short.
 L3 TTA + ensemble of L1/L2 + existing RegionGCN.
Every ladder rung preregistered BEFORE its test evaluation; test evaluated once per rung, all results
committed including failures.

## GATE P5 (pneumonia DISCOVERY): causal-cleaning claim died on a pre-registered random-removal ablation
(honest negative, preserved). Pivot: tiered flag release (91-image consensus core) + measured deltas;
if judged weak, Rule 6 ChatGPT redirection with verbatim log.

## JUDGE PLAN: malaria R7-R10+, pneumonia R3-R10+ - each round: paper PDF attached (her 13:09 rule),
verbatim prompt+response logged, fixes implemented with commit evidence.
## MIGRATION: this repo becomes the standalone home of both projects (code+results+papers+logs), byte-
verified against the main repo; main repo keeps its canonical structure.
