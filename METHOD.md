# Methodology

This analysis evaluates aggregate patterns in civilian unidentified aerial report (UAP) data. The goal is not to identify individual sightings, but to assess whether the overall reporting record exhibits signatures consistent with extraordinary causes or whether it aligns with known phenomena and human observational limits.

All steps below were applied uniformly across the dataset.

---

## 1. Data Union and Deduplication

Multiple public UFO/UAP datasets were combined into a single union dataset.

- Records were standardized to common fields where possible.
- Obvious duplicates (identical date, time, location, and description patterns) were removed.
- Reports with clearly invalid dates (e.g., far-future timestamps) were excluded.

This produced a consolidated dataset of approximately **570,000** reports.

---

## 2. Time Precision Separation

Reports were separated into two categories based on time resolution:

- **Exact-time reports:** sightings with a specific reported time
- **Date-only reports:** sightings with missing, default, or placeholder times (commonly midnight)

This separation prevents artificial clustering caused by default timestamps and allows appropriate handling of each category.

---

## 3. Burst and Spike Control

Two forms of non-informative clustering were addressed:

### Temporal Burst Windows
- Short-duration, high-density reporting windows (minutes to hours) were identified in the exact-time data.
- These bursts are consistent with known mass-observation events (e.g., meteor storms).
- Extreme bursts were flagged and controlled to prevent them from dominating aggregate patterns.

### Publication-Day Spikes
- In date-only data, extreme single-day spikes consistent with batch reporting or database publication effects were identified.
- Only the most extreme outliers were controlled, preserving normal reporting variation.

---

## 4. Time Normalization

Where location information was available, reported times were normalized to approximate UTC using:

- Longitude-based offsets when coordinates existed
- Regional timezone mappings when only administrative locations were available

Uncertainty introduced by coarse timezone inference was tracked conceptually and treated conservatively.

---

## 5. Fireball Cross-Matching

High-confidence atmospheric fireball events were used to test whether these explain a significant fraction of sightings.

- Strict temporal (±60 minutes) and spatial (≤500 km) matching criteria were applied where coordinates allowed.
- Only strong matches were counted to avoid over-attribution.

This step was intentionally conservative and resulted in a very small number of matches.

---

## 6. Residual Calculation

After controlling for:
- burst windows
- publication artifacts
- timestamp issues
- strict fireball coincidences

the remaining reports were treated as a **residual population** for further evaluation.

Approximately **75%** of reports remained after these direct subtractions.

---

## 7. Theoretical Narrowing Using Known Human Factors

Rather than further numerical subtraction, the residual was evaluated against empirically established rates from other fields, including:

- Aviation safety (visual misjudgment rates)
- Psychology and eyewitness research (perceptual and expectation effects)
- Human factors and physiology (night vision, fatigue, environmental distortion)
- Reporting and memory artifacts

These independent research areas consistently show that **70–75%** of ambiguous human-reported observations can be accounted for by normal perceptual and cognitive factors.

Applying these rates provides a bounded estimate of how much of the residual is plausibly explainable without invoking extraordinary causes.

---

## Interpretation Principle

Unclassified or unresolved reports are treated as **limits of data resolution**, not as evidence of unknown objects.

The analysis emphasizes:
- population-level behavior
- statistical structure
- and explanatory boundaries

over individual case interpretation.
