# Frostbloom Waltz

A Genshin Impact–inspired boss fight in one HTML file. You lead a party of two against **Pyrrhos, the Scorched Sovereign**, a Pyro boss:

- **Yukina, the Frostbloom Maiden** (Cryo): a melee sword fighter. Her slashes are physical and only land within reach of the boss (she steps in a little when close). Frostfan Gale (E, 10s cooldown) sends an icy gust from her fan into the boss and frost-infuses her sword for 6s, so slashes apply Cryo. Eternal Winter Waltz (Q, 16s cooldown, needs 60 energy) is 3s of blizzard around her that hits hard, blows away fireballs, and makes her sword 2.2x stronger with longer reach.
- **Mizuha** (Hydro): a long-range support. Her attack is a stream of bubbles that drift to the boss from anywhere but hit lightly (well under half of Yukina's damage). Tide Sprite (E) is a water koi that keeps attacking for 6s even after you switch out, also at low damage. Tidal Lullaby (Q) sends a tide rolling out from her to the cave walls: it hits the boss once, heals both characters 30% + 150 HP, and for the next 3s each of her attacks heals both a little more.

Character and boss art (in-battle sprites, Elemental Burst poses, the boss's normal / attack / burst / defence / downed states, and fireball, eruption, rock-burst and lava-pool effects) is embedded in `index.html` as WebP data. Open `index.html` in a browser to play. There is no build step.

## Controls

| Input | Action |
| --- | --- |
| WASD / arrows | Move |
| Click / J (hold) | Attack. Yukina: sword combo (3 slashes and a spin), must be in reach. Mizuha: long-range bubbles that drift to the boss, light damage |
| 1 / 2 | Switch to Yukina / Mizuha (0.8s cooldown; a downed character can't be picked) |
| E | Elemental Skill (Yukina): Frostfan Gale, an icy gust from her fan into the boss; her sword is frost-infused for 6s |
| E | Elemental Skill (Mizuha): Tide Sprite, a 6s water spirit that keeps firing while the other character is on the field |
| Q | Elemental Burst (Mizuha): Tidal Lullaby, a tide wave that hits once and heals both characters 30% + 150 HP; for 3s after, each of her attacks heals both by 2.5% + 10 |
| Q | Elemental Burst (Yukina): Eternal Winter Waltz, 3s of strong ice wind over a wide area; sword damage x2.2 and damage taken -40% while it lasts |
| Space | Jump: while airborne, ground attacks (shockwaves, fire trails, eruptions, meteors, the charge) miss you |
| Shift (hold) | Run: 65% faster, drains stamina |
| C / Right-click | Dash with i-frames (uses stamina) |
| P / Esc, M | Pause, Mute |

The key legend stays on screen during the fight. Touch controls (joystick and buttons) show up on phones.

## Arena

The fight takes place in **Magma Hollow**, Pyrrhos's lava cave: a basalt platform with glowing fissures ringed by a lava lake with drifting highlights, popping bubbles and two lavafalls, under a ceiling of stalactites, with ash and embers in the air.

## Mechanics

- **Elements:** Cryo and Hydro hits attach their element to the boss (icon over his head).
- **Frozen:** Cryo on a Hydro-affected boss, or Hydro on a Cryo-affected boss, freezes him for 3.2s. He can't be frozen again for 4s after he thaws.
- **Vaporize:** Hydro on his Pyro flames deals 2× damage.
- **Party:** both characters' cooldowns tick while benched. Energy particles give 60% to the benched character. If the active character falls, the other one switches in.

- **Melt:** Pyrrhos is Pyro-affected when he attacks (unless Cryo or Hydro is already on him). Cryo hits then Melt for 1.5× damage.
- **Blazing Aegis:** below 55% HP (and again at 25%) he gains a shield. Elemental hits do 2.5× damage to it (physical slashes do normal damage), and breaking it freezes him for 5.5s.
- **Boss animation:** Pyrrhos breathes while idle, winds up with a "!" cue, lunges into the attack pose for volleys and eruptions, curls into his rock-ball defence form to roll through his charge and while his Aegis is up, flares into his burst form for shockwaves, meteors and spirals, turns icy when Frozen, and collapses when his shield breaks or he's defeated.
- **Attacks:** fireball volleys, a telegraphed charge that leaves fire, eruptions, and shockwave rings you can dash through. Phase II adds a meteor rain and a bullet spiral.
