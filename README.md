# Frostbloom Waltz

A Genshin Impact–inspired boss fight in one HTML file. You lead a party of two against **Pyrrhos, the Scorched Sovereign**, a Pyro boss:

- **Yukina, the Frostbloom Maiden** (Cryo): ice shards, Frostbloom (E) and Eternal Winter Waltz (Q).
- **Mizuha** (Hydro): water orbs, Tide Sprite (E, a water koi that keeps attacking for 6s even after you switch out) and Tidal Lullaby (Q, heals the whole party, then rains healing for 5s).

Character art (the two in-battle sprites and the two Elemental Burst poses) is embedded in `index.html` as WebP data. Open `index.html` in a browser to play. There is no build step.

## Controls

| Input | Action |
| --- | --- |
| WASD / arrows | Move |
| Click / J (hold) | Attack: Frost Shards home in on the boss and always hit (3-hit combo, then a 5-shard finisher) |
| 1 / 2 | Switch to Yukina / Mizuha (0.8s cooldown; a downed character can't be picked) |
| E | Elemental Skill (Yukina): Frostbloom, an ice lotus that locks onto the boss, heals you and drops energy particles |
| E | Elemental Skill (Mizuha): Tide Sprite, a 6s water spirit that keeps firing while the other character is on the field |
| Q | Elemental Burst (Mizuha): Tidal Lullaby heals both characters 30% + 150 HP, then 2.5% every 0.5s for 5s |
| Q | Elemental Burst (Yukina): Eternal Winter Waltz, a 6s blizzard of homing icicles that blocks fireballs and cuts damage taken by 40% |
| Space | Jump: while airborne, ground attacks (shockwaves, fire trails, eruptions, meteors, the charge) miss you |
| Shift (hold) | Run: 65% faster, drains stamina |
| C / Right-click | Dash with i-frames (uses stamina) |
| P / Esc, M | Pause, Mute |

The key legend stays on screen during the fight. Touch controls (joystick and buttons) show up on phones.

## Mechanics

- **Elements:** Cryo and Hydro hits attach their element to the boss (icon over his head).
- **Frozen:** Cryo on a Hydro-affected boss, or Hydro on a Cryo-affected boss, freezes him for 3.2s. He can't be frozen again for 4s after he thaws.
- **Vaporize:** Hydro on his Pyro flames deals 2× damage.
- **Party:** both characters' cooldowns tick while benched. Energy particles give 60% to the benched character. If the active character falls, the other one switches in.

- **Melt:** Pyrrhos is Pyro-affected when he attacks (unless Cryo or Hydro is already on him). Cryo hits then Melt for 1.5× damage.
- **Blazing Aegis:** below 55% HP (and again at 25%) he gains a shield. Cryo does 2.5× damage to it, and breaking it freezes him for 5.5s.
- **Attacks:** fireball volleys, a telegraphed charge that leaves fire, eruptions, and shockwave rings you can dash through. Phase II adds a meteor rain and a bullet spiral.
