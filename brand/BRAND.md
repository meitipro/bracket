# Brand

## The mark

Four bars of decreasing length, with **two of equal length** and a bracket
joining them.

A ranking, and a tie inside it. The tie is the whole family: pretending to
separate two things that are not separable is exactly where consensus breaks, so
the mark shows the **refusal** rather than only the order.

Built on a 100 × 100 grid. Stroke weight 8.5, round caps, corner radius 18. The
tie bracket is lighter, at 3.5, in chalk rather than the accent, so it reads as
annotation rather than as a fifth bar.

- **Clear space:** half the mark height on every side.
- **Smallest size:** 18px alone, 24px locked to the wordmark. Verified — all four
  bars and the bracket stay separable.
- **Never:** a second hue, a gradient, an outline version, a drop shadow, or the
  mark rotated. The geometry carries the meaning.

## Palette

| Token | Hex | Use |
|---|---|---|
| `ink` | `#0C0D10` | the mark's field, any dark surface |
| `chalk` | `#E8E6E1` | the wordmark, primary text, the tie bracket. Never pure white |
| `accent` | `#E0A23C` | the bars, one primary action, one live state |
| `muted` | `#9AA0A8` | secondary text |
| `rule` | `#232830` | hairlines and dividers |

One accent, used sparingly. On the social card it appears exactly three times:
the top bar, the mark, and the footer line.

The accent is distinct from its two siblings on purpose: Crosscheck is violet
`#8B7CF6`, Tolerance is green `#3DD68C`. Same geometry language, different hue,
so the three read as one hand without reading as one product.

## Type

Inter, weights 400 and 700. Tracking tightened to -1.4 on the wordmark and -2.6
at display size. Monospace for anything that is a value rather than a sentence:
`ui-monospace, SFMono-Regular, Menlo, monospace`. The wordmark is always
lowercase.

## Files

| File | What it is |
|---|---|
| `mark.svg` | the mark alone, 100 × 100 |
| `lockup.svg` | mark plus wordmark |
| `social.svg` | 1280 × 640 source |
| `social.png` | export, for Settings → Social preview |

## Re-exporting the social card

```bash
pip install cairosvg
python -c "import cairosvg; cairosvg.svg2png(url='brand/social.svg', \
    write_to='brand/social.png', output_width=1280, output_height=640)"
```

Upload under **Settings → General → Social preview**. GitHub uses it whenever a
link to the repository is shared, including inside a portal submission.
