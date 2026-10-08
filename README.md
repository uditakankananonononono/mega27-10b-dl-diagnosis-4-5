# mega27-10b: diagnoses 4-5 (malaria, pneumonia) - preregistration and judge log only

Status: this repository holds the locked completion preregistration and the first judge-round log for diagnoses 4 (malaria) and 5 (pneumonia). It contains no code, data, results or paper. The planned migration of the projects into this repo (stated in `PREREG.md`) has not happened.

## Where the work is
The malaria and pneumonia projects (CNN + RegionGCN, confident-learning census, papers, judge loops) are in `mega27-10-dl-diagnosis-suite`, directory `subitems_4_5/` (481 tracked files at the time of writing, with its own README and results). Read results there, not here.

## What is in this repo
- `PREREG.md` - completion gates M4/M5 (malaria benchmark beat, label-noise census) and P4/P5 (pneumonia benchmark beat, discovery). It records, as of its lock date, that the pneumonia benchmark was NOT beaten (best committed test accuracy 0.8413 vs published 92.8%).
- `JUDGE_ROUNDS.md` and `judge/` - round 1 (ideation) prompt and response, logged verbatim, with a recorded premise correction: the round was run before the repo audit found 10.4/10.5 already built, so no disease swap was decided.
- `docs/SOURCE_PROVENANCE_GAPS.md` - documentation record of source-term and hash gaps.

## Verified / thin / missing
- Verified: the files above exist at this commit.
- Thin: gate outcomes (M4, M5, P4, P5) are stated in `PREREG.md` as targets or current-state notes from the lock date, not as results; confirm any number in the suite repo before citing it.
- Missing: code, data, results, papers, tests, and the byte-verified migration `PREREG.md` promises.
