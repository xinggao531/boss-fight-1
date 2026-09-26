# Frostbloom Waltz

A Genshin Impact–inspired boss fight in one HTML file. You play **Yukina, the Frostbloom Maiden**, a Cryo catalyst user, against **Pyrrhos, the Scorched Sovereign**, a Pyro boss.

Open `index.html` in a browser to play. There is no build step.

## Controls

| Input | Action |
| --- | --- |
| WASD / arrows | Move |
| Click / J (hold) | Attack: Frost Shards home in on the boss and always hit (3-hit combo, then a 5-shard finisher) |
| E | Elemental Skill: Frostbloom, an ice lotus that locks onto the boss, heals you and drops energy particles |
| Q | Elemental Burst: Eternal Winter Waltz, a 6s blizzard of homing icicles that blocks fireballs and cuts damage taken by 40% |
| Space | Jump: while airborne, ground attacks (shockwaves, fire trails, eruptions, meteors, the charge) miss you |
| Shift (hold) | Run: 65% faster, drains stamina |
| C / Right-click | Dash with i-frames (uses stamina) |
| P / Esc, M | Pause, Mute |

The key legend stays on screen during the fight. Touch controls (joystick and buttons) show up on phones.

## Mechanics

- **Melt:** Pyrrhos is Pyro-affected whenever he attacks. Cryo hits on him then Melt for 1.5× damage.
- **Blazing Aegis:** below 55% HP (and again at 25%) he gains a shield. Cryo does 2.5× damage to it, and breaking it freezes him for 5.5s.
- **Attacks:** fireball volleys, a telegraphed charge that leaves fire, eruptions, and shockwave rings you can dash through. Phase II adds a meteor rain and a bullet spiral.
