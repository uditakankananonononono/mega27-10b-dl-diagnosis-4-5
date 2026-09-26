# MEGA27-10b - ChatGPT Judge Rounds (verbatim log)
Account: her ChatGPT (Free) via cloud browser, config-c, read lease per round.
Standard (her 13:09:44 rule): every weakness round gets the actual paper PDF attached.
Rounds: verbatim prompt + response, decision, implemented fix with evidence.

## ROUND 1 - IDEATION (2026-09-26 16:18-16:20 IST)
Conversation: https://chatgpt.com/c/6ab7a318-347c-83ee-b022-d1b7d7036629
Prompt: judge/10b-round01-ideation-prompt.txt (verbatim)
Response: judge/10b-round01-ideation-response.txt (verbatim, 7644 chars)

### PREMISE CORRECTION (honest log)
This round was run under a stale premise: it asked ChatGPT to SELECT new diseases 4-5, before the
repo audit revealed 10.4 malaria + 10.5 pneumonia were already built in the main suite repo
(subitems_4_5/). The selection question was therefore void. NO disease-swap decision was taken;
malaria + pneumonia remain diagnoses 4-5.

### Salvageable content (applies only if expansion items 10.6-10.7 are assigned here)
- Judge killed OASIS-1 MRI as a weak benchmark target (leakage-inflated published numbers, 3/5).
- Judge killed Kaggle-PCOS-style small tabular datasets (2/5).
- Judge backed transcriptomic diagnosis (sepsis GSE65682, AD blood GSE63060; both verified real on GEO).
- General framework adopted: "a beat is only defensible if the baseline is reimplemented or evaluated
  under the exact same split, preprocessing, and metric; a discovery must be a biological/clinical
  insight, not 'our model is better'." - this standard is applied to Gates M4/M5/P4/P5 in PREREG.md.
