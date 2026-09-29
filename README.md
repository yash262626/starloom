# ✦ STARLOOM — Weave Light. Bind the Void.

[![Play Live](https://img.shields.io/badge/🎮_Play_Live-Open_STARLOOM-00C7B7?style=for-the-badge)](https://yash262626.github.io/starloom/)

An arcade **loop-drawing game** for the browser. Steer a spark, leave a ribbon of light behind you, and cross it to close a loop. Every shadow inside the loop is *bound* and turns into score. Survive escalating phases, chase combos and unlock new ribbons.

Everything lives in a single `index.html`: no dependencies, no build step, no server, no external assets.

**Play:** open `index.html` in any modern browser (desktop or mobile), (the live version above is hosted by the author; re-hosting is not permitted, see License).

---

## How to play

1. **Move**: the spark follows your cursor or finger, trailing a ribbon of light.
2. **Loop**: cross your own ribbon to close a loop. Every shadow inside is bound.
3. **Combo**: more shadows in one loop means a bigger bonus. Bind quickly to raise your multiplier (×1, ×2, ×3…) and extend your chain.
4. **Nova**: collecting stardust charges your Nova. Unleash it to bind everything around you.

## Shadows (enemies)

| Shadow | Behaviour |
|---|---|
| **Drifter** | Slow, hunts your spark |
| **Swarm** | Tiny packs, perfect combo fodder |
| **Dasher** | Takes aim, then lunges |
| **Warden** | Shielded, needs two loops |
| **Shear** | Slices your ribbon on contact |
| **Titan** | Colossal, must be enclosed completely |
| **Golden Wisp** | Harmless, fleeting and very valuable |

## Power-ups (touch them or loop them)

| Power-up | Effect |
|---|---|
| **Long Ribbon** | Much longer trail |
| **Aegis** | Absorbs one hit |
| **Chrono** | Slows every shadow |
| **Double** | 2× score for a while |
| **Core** | Restores a life |

## Controls

| Input | Action |
|---|---|
| Mouse | Steer, the spark chases your cursor |
| `W` `A` `S` `D` / arrow keys | Steer with the keyboard |
| `Space` / right-click | Unleash Nova when charged |
| `P` / `Esc` | Pause |
| `M` | Mute |
| `R` | Restart (from the pause screen) |
| Touch | Drag anywhere like a trackpad; double-tap or tap ✦ for Nova |

## Game systems

- **Phases:** difficulty and enemy mix escalate as you survive; each phase gets an intro banner and a progress meter.
- **Objectives:** per-run goals to complete for extra stardust.
- **Ranks:** every run ends with a rank and a results screen (score, bound shadows, best loop, best chain, phase reached, time survived, near misses, objectives, stardust earned).
- **Stardust & the Loom:** stardust from each run is woven into your Loom, where you unlock and equip new ribbons.
- **Trophies:** achievements tracked across runs.
- **Stats:** best score, best chain and biggest loop shown on the main menu.
- **Persistence:** progress is saved in the browser via `localStorage`, with a safe in-memory fallback when storage is blocked (private mode, etc.).

## Settings

Sound effects (procedural synth), music (generative ambient score), volume, screen shake, high-quality effects (turn off on older devices), touch steering (Drag or Direct), coach hints for new players, and a reset-progress option.

## Tech notes

- Vanilla **HTML + CSS + JavaScript**, rendered on `<canvas>`.
- All audio is generated in the browser (Web Audio), so there are no audio files.
- Responsive and touch-friendly; design tokens live in CSS custom properties.
- Single file, so it is easy to fork, host or embed.

## License

This project is source-available under the [Yash AIL Source-Available License](LICENSE): you may view, copy and modify it for personal, educational and non-commercial local use. **Deploying/hosting it online and selling it are not allowed.**

---

© 2026 Yash AIL — All Rights Reserved
