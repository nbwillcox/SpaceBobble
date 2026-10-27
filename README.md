# SpaceBobble

A free, retro sci-fi bubble-blowing arcade game in chunky pixel art with 8-bit music, a head nod to the classic NES-era bubble platformers. You are a little astronaut with a bubble blaster: trap the alien invaders in bubbles, pop them for fruit-style space snacks, and fight your way through 100 single-screen levels across 10 worlds, with a boss at the end of every world.

**Play it in your browser:** https://nbwillcox.github.io/SpaceBobble/

Everything is generated in code: all sprites, tiles and backdrops are pixel art built at startup by a tiny software rasteriser, and all sound effects and music are synthesized with the Web Audio API. There are no image or audio files and no build step. A sibling of [SpaceContra](https://github.com/nbwillcox/SpaceContra), [FSpaceZero](https://github.com/nbwillcox/FSpaceZero), [SpaceDug](https://github.com/nbwillcox/SpaceDug) and the rest of the Space series, with the same look and feel.

## Controls

| Action | Keyboard | Gamepad |
| --- | --- | --- |
| Move | `←` `→` or `A` `D` | left stick / d-pad |
| Jump | `Space`, `Z`, `K`, `↑` or `W` | `A` / `B` |
| Drop down a level | `↓` or `S` + jump | stick / d-pad down + `A` |
| Blow a bubble | `X`, `J`, `L`, `Shift` or left mouse click (hold to keep blowing) | `X` / `Y` / `RB` |
| Pause | `P` or `Esc` | `Start` |

Menus work with the arrow keys and `Enter`, the mouse, or a gamepad. The playfield stretches to the window: ultrawide screens simply get a wider room (up to 80 columns).

### On a phone or tablet

Play in landscape. A floating stick on the left runs (down plus jump drops through a platform); **JUMP** and **BLOW** are on the right. The pause button opens the menu. The on-screen controls appear on touch devices automatically; Settings has size, opacity and a left-handed layout. Use your browser's *Add to Home Screen* to install it as a full-screen app.

### Controller

Plug in a gamepad and it just works: the stick or D-pad runs, **A** jumps, **X / B / RT** blows a bubble, **Start** pauses. In menus the D-pad / left stick moves the highlight, **A** selects, **B** goes back and **Start** plays or resumes. **Settings -> Controller** has a dead-zone slider and lets you remap every button.

## How to play

- **Blow bubbles at aliens** to trap them. A trapped alien floats up and, if you wait too long, bursts free and comes back **angry** (faster). Touch the bubble first to pop it: the alien turns into a space snack worth points, and chain-popping aliens multiplies the bonus.
- **Bubbles are platforms.** Jump on top of an empty bubble to ride it upward; touch one from the side or below to pop it. Bubbles pop their neighbours in a chain reaction.
- **Special bubbles** float by now and then. Pop one to unleash a **coolant wave** (rolls along the floor), **arc bolts** (zap sideways) or **plasma fireballs** (bounce around) that clear aliens.
- **EXTEND:** catch the six letter bubbles E-X-T-E-N-D in a world for an extra life and a big bonus. Complete the word in **all ten worlds** to unlock the secret true ending.
- **Candies** grant a timed boost: speed, rapid fire or long-range bubbles. A rare **warp ring** skips up to three levels.
- **Don't dawdle:** after a while the aliens turn angry (HURRY UP!), and later the **Void Maw** starts hunting you.
- **Levels:** 100 single-screen rooms in 10 worlds (Asteroid Mine, Space Station, Ice Moon, Lava Planet, Alien Jungle, Crystal Caverns, Cyber City, Derelict Ship, Nebula Garden, Black Hole Core). Some rooms have **low-gravity pockets**. Every 10th level is a **boss**: wear it down with bubbles and special blasts. Beat the last one to finish the game.
- **Difficulty:** Easy, Normal or Hard when you start (lives, continues, alien speed, trap time and the hurry-up timer change). Arcade-style top-10 high scores with three-letter initials and a limited number of continues. Scores, settings and progress are saved in your browser.

## Run locally

It is plain HTML/CSS/JS. Either open `index.html` directly, or serve the folder:

```bash
python -m http.server 8000
```

then visit http://localhost:8000. Handy URL parameters: `?play=1` skips the title and starts on Normal (0 Easy, 1 Normal, 2 Hard), `&level=N` starts at level N, and `&god=1` makes you invulnerable.

## License and attribution

Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): free to play, share and remix **non-commercially**, as long as you give credit and **link back to this repository**: https://github.com/nbwillcox/SpaceBobble

This is an original game inspired by classic arcade platformers. It uses no assets, names or code from any existing game.
