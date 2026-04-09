# Grendel Muðbona

**The Mouth-Slayer of Heorot** — a Pac-Man style arcade game set in the world of *Beowulf*, designed for advanced Old English classes.

You play as Grendel, the *nihtgenga* (night-walker), raiding Heorot and devouring sleeping Geats. In the second level, you play as Grendel's mother (*Grendles mōdor*), returning to avenge her son.

## Playing the Game

Open `index.html` in any modern browser. No server or build step required.

If GitHub Pages is enabled, play directly at:
**https://caedmon5.github.io/muthbona/**

### Controls

| Key | Action |
|-----|--------|
| Arrow keys / WASD | Move Grendel through Heorot |
| P | Pause / unpause |
| Enter / Space | Advance through title and intro screens |

The game begins on the GEARO! (Ready!) screen. Press any direction key to start moving — Grendel will not move until you choose a direction.

## The Poem

The game is loosely based on Beowulf lines ~740–745a and ~1900ff, where Beowulf recounts to Hygelac how Grendel attacked Heorot and devoured Hondscīo. The intro screen displays the Old English:

> Þa com of mōre &ensp; under misthleōþum  
> Grendel gongan, &ensp; Godes yrre bær;  
> mynte se mānsceaþa &ensp; manna cynnes  
> sumne besyrwan &ensp; in sele þām hēan.

*Then came from the moor, under misty cliffs, / Grendel walking, bearing God's anger; / the evil ravager meant to ensnare / some of mankind in that high hall.*

## Gameplay

### Objective

Devour all the sleeping Geats (gold dots) in Heorot while avoiding the warriors who patrol the hall. Collect the **glōf** (Grendel's magical glove — the green pulsing power-ups) to temporarily frighten most enemies.

### The Arm-Ripping Mechanic

Grendel has **two arms** (displayed in the HUD as "Earmas"). Unlike traditional Pac-Man lives, losing an arm does not reset the game — you keep playing with a bloody stump visible on your sprite, and you flash with brief invulnerability for 2 seconds. Lose both arms and the game ends, echoing the climax of the poem: *Bēowulf hæfde Grendles hand!* (Beowulf had Grendel's hand!)

### Characters

#### Grendel (Player — Fitt I)
Green humanoid figure with glowing eyes and prominent clawed arms. Moves through Heorot devouring the sleeping warriors. When an arm is ripped off, the sprite shows a bleeding stump.

#### Grendles Mōdor (Player — Fitt II)
Grendel's mother, darker green with long dark hair. She arrives to avenge her son. Plays the same maze with increased difficulty and different Old English phrases drawn from the mother's section of the poem (*wrecend gīt leofes*, *mere-wīf mihtig*, etc.).

#### Bēowulf (Blue warrior with sword)
**Always lethal.** The hero of the Geats hunts Grendel relentlessly with direct-chase AI. He is never frightened by the glōf — he cannot be eaten. Contact rips off one of your arms. He is the most dangerous enemy in the game, just as in the poem.

#### Wulfgār (Red warrior with spear)
The herald of Hroðgar. Uses ambush AI — he targets the space four tiles ahead of Grendel, trying to cut you off. Can be eaten when frightened by the glōf. Contact costs an arm.

#### Unferð (Pink warrior with sword)
The skeptic of the poem. Every encounter with Unferth is a **50/50 coin flip**: either you overcome him (*Unferð ofercumen!*) for 300 points, or he withstands you (*Unferð wiðstōd!*) and rips off an arm. When frightened by the glōf, he can be eaten normally.

#### Hrōðgār (Grey figure with crown, white beard, walking staff)
The aged king of the Danes. He is slow-moving (the slowest enemy), always flees from Grendel, and can be caught even without the glōf for **500 points**. His sprite features a golden crown, long wispy white beard, forehead wrinkles, and a stooped posture — the hoary old king of the poem.

#### Wēalhþēow (Gold-dressed queen with mead cup)
The *freoðuwebbe* (peace-weaver). She patrols the hall carrying her mead cup. If she catches Grendel, she **tames** him — slowing his movement to half speed for 4 seconds (*Wēalhþēow getemode þē — The queen tames you!*). She is not lethal, but the slowdown leaves you vulnerable to the warriors. She is never frightened by the glōf.

### Special Victims

Two sleeping warriors are worth extra points and are highlighted on the maze with pulsing amber figures and name labels:

- **Hondscīo** (200 pts) — The Geat that Grendel devours first in Beowulf's account to Hygelac. *Hondscīo forswealg!*
- **Æschere** (200 pts) — Hrothgar's beloved counselor, killed by Grendel's mother. *Æschere ābiten!*

### Power-Ups: The Glōf

The four green pulsing orbs are the **glōf** (Grendel's magical glove/bag from the poem). Collecting one frightens most enemies, causing them to turn blue and flee — you can eat them for escalating points (200, 400, 800, 1600). Exceptions: **Bēowulf is never frightened**, and **Wēalhþēow is never frightened**.

## Old English in the Game

The game is designed to immerse students in Old English vocabulary and phrases. During gameplay, eating Geats triggers short OE phrases drawn from the poem:

| Old English | Translation |
|-------------|-------------|
| slǣpende rinc | sleeping warrior |
| bānhūs gebræc | broke the bone-house (body) |
| synsnǣdum swealh | swallowed in sinful morsels |
| fēt ond folma | feet and hands |
| blōd ēdrum dranc | drank blood from veins |
| līc eall forswealg | swallowed the whole body |
| gryre lēoda | terror of the people |
| dēaðscua | death-shadow |
| wæl rēahte | piled the slaughter |
| heoro drēorig | sword-bloody |
| gūðrinc monig | many a war-man |

In Fitt II (Grendel's Mother), different phrases appear: *wrecend gīt leofes* (avenger of a loved one), *mōdor Grendles* (Grendel's mother), *mere-wīf mihtig* (mighty mere-woman), etc.

### HUD Labels

| English | Old English | Meaning |
|---------|------------|---------|
| Score | Wælfyll | Slaughter-count |
| Level | Fitt | Section (of a poem) |
| Arms | Earmas | Arms |

## Levels

- **Fitt I** — Play as Grendel raiding Heorot. OE intro from lines 740–745a.
- **Fitt II** — Play as Grendles Mōdor avenging her son. Transition screen with OE text: *Grendles mōdor, ides, āglǣcwif, yrmþe gemūnde...* ("Grendel's mother, a woman, a monster-wife, remembered her misery..."). Increased enemy speed, shorter frighten duration.
- Further fitts alternate between Grendel and his mother with increasing difficulty.

## Branches

- **`main`** — Humanoid pixel-art sprites, arm-ripping mechanic, Wealtheow, Grendel's Mother level
- **`pac-man-style`** — Classic Pac-Man/ghost-shape aesthetic with traditional lives system

## Technical Details

- Single HTML file, no dependencies, no build step
- HTML5 Canvas rendering at 60fps
- All audio synthesized via Web Audio API (no external files)
- Responsive scaling to fit any browser window
- High scores saved to localStorage

## Credits

Created for use in advanced Old English courses.

Built with [Claude Code](https://claude.ai/claude-code).
