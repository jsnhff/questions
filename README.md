# will happiness find me?

A durational, self-running web piece: questions fade up out of the black,
hold, and fade back — endlessly, never answered.

**Live:** https://willhappinessfind.me

After Peter Fischli & David Weiss, *Will Happiness Find Me?* / *Questions*
(2000–2003) — hundreds of handwritten queries projected in a dark room.
Form after Rafaël Rozendaal's browser-native artworks. By Jason Huff (2026).

## What it is

A single, self-contained `index.html` — vanilla JavaScript and a 2D canvas,
no libraries, no build step.

- Questions are dealt from a pool of ~800 and rendered on their own gently
  **wavy, tilted baselines**, so where they cross they stay legible.
- Each fades **black → colour → black** (slow to appear, quick to fade),
  composited as light so overlaps glow rather than collide.
- Colours come from a five-hue palette; never more than two of one hue on
  screen at once.
- Placement is **blue-noise** (even, no grid); the field breathes at ~8
  questions, never more than 11.
- A **no-repeat deck**: a question returns to the back of the shuffled deck
  when it leaves, so nothing repeats until the rest of the pool has cycled.
- **Responsive**: sizes itself from phone to desktop. Longer questions are a
  wide-screen treat — on small screens they sit out so nothing shrinks.

## The questions

The pool lives inline in `index.html`. It mixes the register of the original —
existential, trivial, absurd, empirical, metaphysical — written for this time:
the AI-and-human present alongside the timeless business of being a person.

`questions.json` is an optional live override: if present and non-empty, the
piece uses it instead of the built-in pool (a hook for a future generator).
Empty by default, so the built-in pool is used.

### Adding questions

Questions are collected over time — including out in the world, at parties,
from whoever's asking. New ones are de-duplicated against the pool and folded
in. Suggestions welcome.

## Develop

It's one file. Open `index.html` in a browser. That's the whole toolchain.

## Credits & license

Concept after Fischli/Weiss; form after Rozendaal. Questions and code © Jason
Huff. Homage, not affiliated with the artists or their estates.
