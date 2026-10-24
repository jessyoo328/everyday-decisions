# Metacognitive Uncertainty, Study 2

Study page for Study 2 (version s2-1.0.0). Everything is in `index.html`.

- **Live link:** https://jessyoo328.github.io/mu-study2/
- **Prolific link:** add `?PROLIFIC_PID={{%PROLIFIC_PID%}}&STUDY_ID={{%STUDY_ID%}}&SESSION_ID={{%SESSION_ID%}}`
- **Test run:** add `?test=1` (rows are saved with `is_test = true`, and timers are skipped)

## Design

Five everyday situations per person, in random order. For each: a 4-item metacognitive uncertainty scale, two first-order ratings (knowable, chance), certainty about the outcome (0–100), a binary choice between a find-the-cause action and a hedge action (main DV), and felt knowledge of the domain (1–7). Measure order (MU first or choice first) is randomized between people. Then the 15-item Need for Closure scale (Roets & Van Hiel, 2011), demographics, a careful-answering check and a debrief.

## Data

Answers are saved on submit to the Supabase project "Metacognitive Uncertainty", table `study2_responses`. The page's key can only insert rows (row-level security); it cannot read them. The view `study2_long` has one row per participant x situation.

## Before launch

1. Set `COMPLETION_CODE` in `index.html` to the code Prolific gives you.
2. IRB approval for these materials.
3. On Prolific, limit devices to desktop (the page also blocks phones and tablets).
