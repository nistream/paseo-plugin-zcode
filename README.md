# PR #3 visual comparison

Supporting images for https://github.com/lianxin255/paseo-plugin-zcode/pull/3.

- `after-sidebar.png` and `after-usage-card.png` are the original screenshots supplied by the contributor, copied without editing.
- `before-sidebar.png` and `before-usage-card.png` are HTML/CSS reconstructions, NOT historical captures from an unpatched application. Each has a visible reconstruction label. Their standalone HTML sources are included in `reconstruction/`.
- The reconstruction reflects the pre-fix parser at upstream commit `36c58eee3a856eead23cf93134e7aec1aa941920`: both CREDIT_LIMIT entries fall back to `id: credit_limit`, `label: CREDIT_LIMIT`, an empty short label and `summary: false`.
- Percentages and reset countdowns are deliberately held constant against the supplied after screenshots. Layout is approximate. The before sidebar illustrates the old default selection / no ZCode pins, not every possible user pin configuration.
- Sidebar pins are device-local preferences. `summary: true` supplies defaults until customized; existing custom selections may still require explicitly pinning the corrected windows. These images do not imply that the patch changes a user's saved preferences.
- The same semantic quotas now map to `token_5h` / `5-hour` / `5h` and `token_week` / `Weekly` / `wk`. Quota counters and reset calculations are unchanged.

The visuals are hosted on a separate documentation branch in the contributor's fork; the code PR remains focused on its original three files.
