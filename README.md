# INFER Study Beta — Treatment Group 2

## Study Condition: INFER chain prompt (no tutorial video)

This is the **Treatment 2** version of the INFER 4-video experiment.
Participants receive INFER chain-prompt feedback on Videos 2 & 3 (identical prompts to Alpha), but do **not** watch a tutorial video.

### Video Configuration

| Video | Tutorial | INFER Feedback | Notes |
|-------|----------|----------------|-------|
| Video 1 | ❌ | ❌ | Reflection only (baseline) |
| Video 2 | ❌ | ✅ chain | Chain-prompt INFER feedback |
| Video 3 | ❌ | ✅ chain | Chain-prompt INFER feedback |
| Video 4 | ❌ | ❌ | Reflection only (post-test) |

### Study Flow

```
Welcome/Consent → Login → Pre-Survey (mandatory)
    ↓
Video 1: Watch → Reflect → Submit → Post-V1 Survey
    ↓
Video 2: Watch → Reflect → INFER chain feedback → Revise → Submit → Post-V2 Survey
    ↓
Video 3: Watch → Reflect → INFER chain feedback → Revise → Submit → Post-V3 Survey
    ↓
Video 4: Watch → Reflect → Submit → Post-V4 Survey
    ↓
Post-Survey (mandatory) → Thank You
```

### Difference from Alpha and Gamma

- **vs Alpha (Treatment 1)**: Beta does not show a tutorial video before Video 2. Both use the same INFER chain prompt.
- **vs Gamma (Control)**: Beta uses the INFER chain prompt — binary classification of every reflection window into Description / Explanation / Prediction, then a weighted feedback prompt over those analysis results (max_tokens=2000). Gamma uses a single-shot general prompt with no classification.

### Deployment

Static site on Render. URL: `infer-study-beta.onrender.com`
Data: shared Supabase project (distinguished by `treatment_group = 'treatment_2'`).
