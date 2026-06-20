# Market Overlay v2.1

v2.1 adds Japanese equities/JPY, opt-in GitHub update notifications, Yahoo previous-close correction, clearer performance/treemap status, and a major internal responsibility split while preserving the single Windows application.

## Highlights

- Japanese `.T` symbols and JPY cash/cost basis conversion
- `Heatmap` terminology migrated to `Treemap` with legacy state compatibility
- Stable GitHub Release update checks with per-version ignore
- Conditional Yahoo intraday fallback when the previous daily close is missing
- Visualization, overlay, worker, and lifecycle modules separated
- v2.0 state and backup compatibility regression coverage

## Installer SHA-256

```text
514355869C9A12A8DCC2AE8BA4CEE14C1C07E121481E6143C5917D7AB91EBF37
```

## Notes

- User data remains in `%APPDATA%\MarketOverlay` during an update install.
- The app does not automatically download or install updates.
- This is an unsigned personal build; Windows SmartScreen may show a warning.
