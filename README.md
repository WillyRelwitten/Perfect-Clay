# Perfect Clay v1.0

Side-on 2D skeet toy. **Hitting the clay is easy. A PERFECT shot is strict and celebrated.**

Open `index.html` in a browser. No build step.

Repo: https://github.com/WillyRelwitten/Perfect-Clay

## The rule (do not loosen)

- **HIT** — shot overlaps the clay. Clay breaks. 10 points. Normal break. No slow-mo.
- **PERFECT** — all three:
  1. Clay center inside the small gold core
  2. Shot taken in the crossing window (warm vertical band)
  3. Follow-through: the bead is still moving through the bird (rightward, above speed threshold)
- Stopping or reversing the swing caps the shot at HIT even on a center break.
- Difficulty lives in Perfect, not in missing the clay.

## Juice

Perfect only: super slow-mo shatter + full-screen color wash.

Non-perfect shots: ghost of the ideal intercept + short callout  
`BEHIND / AHEAD / HIGH / LOW / EARLY / LATE / STOPPED SWING`

## Modes

- **Practice** — clays keep coming. Running points / hits / perfects / perfect%.
- **Set of 7** — seven birds, then a scorecard. Replay or return to practice.

## Controls

- Mouse swings the barrel (inertia)
- Click fires one shot
- `P` practice · `7` set of 7 · `R` restart · `Esc` / `M` menu

## Constants to tune (in `index.html`)

```
HIT_RADIUS = 30
PERFECT_RADIUS = 7
FOLLOW_MIN = 220
CROSS_MIN / CROSS_MAX = 0.42 / 0.68
HIT_PTS = 10
PERFECT_PTS = 50
```

## Bot hooks already in code

```
// BOT: second flight path
// BOT: sound
// BOT: tighter core
```

Read `BOTS.md` before changing the game.
