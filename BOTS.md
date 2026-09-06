# Direction for bots — Perfect Clay

Work in this repo: **https://github.com/WillyRelwitten/Perfect-Clay**

This is v1.0 of a one-idea skeet game. Refine it. Do not replace the idea.

## One idea

Breaking the clay is easy. A PERFECT shot is strict, rare, and celebrated.

## Non-negotiable

- Clays are easy to break. Most shots that touch the clay count as a HIT.
- PERFECT is not “also hit the clay.”
- PERFECT requires ALL of:
  1. clay center inside a small core (much smaller than the hitbox)
  2. shot taken in the intended crossing window (the warm band)
  3. follow-through: aim point still moving through the clay at fire
- If the swing is stopped or reversing on fire, cap at HIT even on a center break.
- Player must see WHY a HIT was not PERFECT (ghost + callout).
- Perfect juice: super slow-motion shatter AND a full-screen color wash. Hits do not get this.
- Hits still award points.

## What v1.0 already is

- Single `index.html`, canvas, no build, no required art.
- Side-on 2D. Mouse swings barrel with inertia. Click = one shot. Hitscan bead vs clay.
- One station, one family of left-to-right flight paths, one shot per clay.
- Practice (endless) and Set of 7 with a scorecard.
- Visible crossing window, gold perfect core, faint hit radius.

## Do not add unless asked

Campaign, shops, multiple guns, wind, true pairs, accounts, particle-systems-as-content, story, extra stations as filler.

Do not make the clay tiny as the only way to make the game “hard.”

## Good next passes

- `// BOT: second flight path` — incoming / outgoing / quartering, still one bird at a time
- `// BOT: sound` — pull call, break, perfect sting
- `// BOT: tighter core` — only after playtest, keep HIT generous
- Cleaner barrel sprite, better shatter, hold-bead option
- Keep the scorecard honest: hits, perfects, perfect%, callouts

## Done when

- A casual player can break most clays without trying.
- They cannot rack Perfects without aiming the core and swinging through.
- A Perfect is obvious: world slows, screen changes color.
- A non-perfect hit tells them why in one glance.

## Code shape

Keep sections readable: input, swing/gun, clay, scoring, feedback/juice, modes, loop.  
Leave the BOT comments. Restate Hit vs Perfect in README if you change constants.
