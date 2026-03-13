# AIS C Walking Recovery Bedside Score

Static web implementation of a bedside clinical prediction rule (CPR) for one-year walking recovery in AIS C spinal cord injury.

## Summary

This tool reflects the manuscript:
`A bedside score predicts one-year walking recovery in AIS C spinal cord injury: a multisite cohort study.`

- Cohort: retrospective Spinal Cord Injury Model Systems (SCIMS) data, Jan 2000-May 2019, across 12 centers
- Sample: 1,414 adults initially classified as AIS C
- Outcome: one-year walking recovery composite (indoor 150 ft, one street block outdoors, one flight of stairs)
- Core predictors: lower-extremity myotome strength (L2, L3, L4, S1 at >=3/5) and age thresholds (>=50, >=65)
- Bedside score points: `L2 +1`, `L3 +2`, `L4 +1`, `S1 +1`, `Age >=50 -2`, `Age >=65 -5`
- Interpretation thresholds: `>3 = Likely Walk`, `<-3 = Likely No Walk`, otherwise `Uncertain`

## Repository Purpose

This repository contains a standalone HTML interface to calculate and display the bedside score for clinical/research workflow support.

## Deployment

Configured for static hosting (Netlify + GitHub workflow).

- Entry file: `index.html`
- Publish directory: project root (`.`)
- Netlify config: `netlify.toml`

## Files

- `index.html` — deploy entry page
- `ais-c-walking-cpr-refined.html` — original working file snapshot
- `netlify.toml` — Netlify deploy configuration
