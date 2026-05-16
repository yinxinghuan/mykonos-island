# Alter Isle

A sandbox for your alter self — a zen isometric island builder in
the AlterU collection. Drop blocks onto a 14×14 grid and a tiny village
arranges itself in front of you. No goal, no score; just the
puzzle-piece pleasure of placing things until they look right.

Forked from the lovely
[boona13/mykonos-island-voxels](https://github.com/boona13/mykonos-island-voxels)
and re-skinned to the AlterU brand. The full PNG asset pack, the
isometric renderer, and the touch-first input model are upstream's
work — credit there.

## What's different from upstream

- Re-skinned UI chrome to AlterU palette: bone background, coral as
  the "warm self" accent, violet as the "alter self" accent.
- AlterU watermark at the canonical `/img/aigram.svg` slot.
- Light Aigram integration (`src/aigram.js`) — greets the player by
  name when embedded in Aigram, no-ops everywhere else.
- Namespaced storage key (`alteru.alter-isle.save.v1`) so saves don't
  collide with upstream if both are open in the same browser.
- `meta.json` for the AlterU publish pipeline.

The asset pack itself is untouched — the sun-bleached look reads as
"warm AlterU" already, and pre-rendered PNGs aren't easy to recolour
without losing the painterly quality.

## Run it

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

No build step. Pure ES modules.

## Controls

Same as upstream — see the in-game `?` panel.

## License

MIT (inherited from upstream — see `LICENSE`).
