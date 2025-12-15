# Data Sources

This analysis is based entirely on publicly available datasets. No classified, proprietary, or restricted data were used.

## Primary Dataset: Civilian UAP / UFO Reports

Multiple public UFO/UAP sighting databases were combined into a single union dataset.

**Key characteristics:**
- Approximately **570,000** total reports after cleaning and deduplication
- Time span: **~1900 to 2024**
- Global coverage, with higher density in regions with greater population and reporting infrastructure
- Civilian reports only

**Common fields include:**
- Date and (when available) time of sighting
- Location (country, state, city; coordinates when provided)
- Free-text description
- Source database identifiers

Known data quality issues include:
- Missing or default times (e.g., midnight placeholders)
- Inconsistent location precision
- Occasional erroneous future dates (excluded from analysis)

---

## Supporting Datasets

These datasets were used to test specific explanatory hypotheses at an aggregate level.

### Atmospheric Fireballs
- Source: NASA CNEOS fireball event catalog
- Used to identify high-confidence atmospheric entry events
- Cross-matched using strict temporal and spatial criteria where possible

### Satellites
- Source: UCS Satellite Database (multiple public snapshots)
- Used to assess satellite population growth and orbital class trends over time
- Evaluated at a population level, not via event-by-event visibility modeling

### Asteroids / Near-Earth Objects
- Source: Public NASA/JPL-derived asteroid datasets
- Used for macro-scale temporal context only

### Meteorites
- Source: Meteoritical Society landing catalog
- Used to assess rarity and spatial distribution of recovered meteorites

### Weather
- Source: Public annual weather and climate summary datasets
- Used as a coarse sanity check against climate-driven reporting trends

---

## Data Handling Notes

- All datasets were treated descriptively and statistically.
- No single dataset is assumed to be complete or authoritative on its own.
- Results depend on aggregate behavior across datasets, not on individual records.

The limitations of these data sources are discussed explicitly in `LIMITATIONS.md`.
