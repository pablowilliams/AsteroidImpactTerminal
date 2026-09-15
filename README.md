# Close Approach Desk

A browser-based scenario desk for reviewing a small, fixed catalogue of near-Earth objects. It focuses on inspectable assumptions: the selected object, propagation horizon, random seed and simulated uncertainty paths remain visible throughout the workflow.

## What it demonstrates

- Deterministic scenario generation with selectable path counts and horizons.
- Object-level comparison using close-approach distance, MOID-derived indicators and Torino/Palermo context.
- Keyboard-accessible tables, controls and text alternatives for charts.
- A deliberately labelled synthetic snapshot that works without API keys.

The numerical series are synthetic teaching data. This is not an impact-warning service and must not be used as an alternative to JPL Sentry or ESA NEOCC.

## Run locally

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000`. The published version is available through GitHub Pages.

## Engineering note

This project reuses a deterministic scenario kernel also exercised in four sibling studies. The domain adapter, terminology, data schema and specialist panels are specific to close-approach review; the shared kernel is intentionally disclosed rather than presented as five unrelated implementations.
