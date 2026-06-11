# Combo Guard website

Static marketing site plus docs for [@Combo_Guard_bot](https://t.me/Combo_Guard_bot). No build step, no dependencies.

- `index.html` - landing page
- `docs.html` - setup guide and full options/command reference
- `fonts/` - self-hosted Outfit + JetBrains Mono
- `assets/` - logo (PNG + WebP) and the hero video

## Preview locally

```
python -m http.server 8742
```

Then open http://localhost:8742

## Notes

- All CTAs point to `https://t.me/Combo_Guard_bot?startgroup=true` (the
  `?startgroup=true` opens Telegram's "add to group" picker). Search and
  replace `Combo_Guard_bot` across both HTML files if the username ever changes.
- Logo assets are generated from the master griffin art (cropped to the disc,
  rim faded with a radial alpha mask); the generator script lives in the
  private bot repo. Bump the `?v=` query on logo URLs after regenerating.
- The hero video plays inside a circular mask; users with reduced-motion
  enabled get the static logo instead.
- Sample numbers in the Watchtower report panel are illustrative example
  output, not live stats.
