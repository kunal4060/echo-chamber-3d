ECHO CHAMBER 3D — CTRL+PLAY 2026 (Gamathon) submission
=====================================================
First-person 3D horror. You are alone in a pitch-black abandoned laboratory.
Your sonar pulse reveals the maze — but everything you reveal, IT hears.

HOW TO RUN (fully offline, no internet needed)
--------------------------------------------
1. Keep `echo-chamber-3d.html` and `three.min.js` in the SAME folder.
2. Double-click `echo-chamber-3d.html` (any modern browser: Chrome/Edge/Firefox).
3. Click the page, then press ENTER to begin.

CONTROLS
--------
WASD / arrows .... move (mouse to look once pointer is locked)
SHIFT ............ move quietly (less noise)
Z ................ crouch (quieter still)
SPACE ............ sonar pulse — reveals nearby walls/objects for 2.5s,
                   BUT the sound may attract the creature (4s cooldown)
                   TIP: stand still 10s first for a softer "grace" ping
Double-tap+hold.. sprint (fast but loud, drains stamina)
  movement key
F ................ flashlight on/off (drains battery ~3 min; recharges off)
                   WARNING: the specimen can SEE the beam — light feeds it
Q / click ........ throw a distraction 4 tiles ahead (3 total)
G ................ drop a radio lure (2 total, ticks for 12s)
E (near note) .... read lab notes + recovered audio logs
C ................ security camera view (cycles 5 cams, ESC exits)
                   you see IT live — but you stand still while watching
X ................ inject adrenaline (10s +40% speed, no stamina drain;
                   30s cooldown; the hiss is audible)
M ................ tactical map (fog of war — only visited areas shown)
N ................ mute
R ................ restart (keycards are kept)
ENTER ............ start / advance screens
ESC .............. pause / exit camera view

EXITS (all need 3/3 keycards)
-----------------------------
MAIN ............. east wing — closest to the specimen's nest
VENT ............. north, inside the SECURITY room — fast, but it hears metal
SERVICE .......... south tunnel — long walk, quiet route

SPEEDRUN
--------
The clock starts when you leave the intro and stops at the exit.
Best time per difficulty is saved on this machine; the win screen
tells you which exit you used.

DIFFICULTY (title screen, LEFT/RIGHT arrows)
-------------------------------------------
EASY (GUIDED) .... slower specimen, softer pings, brighter keycards
NORMAL (STANDARD)  the intended hunt — fair, but it is listening
HARD (NIGHTMARE) . faster, sharper-eared specimen. For those who like dying.

GOAL
----
Find all 3 keycards, then reach ANY exit (they turn green when unlocked):
MAIN (east), VENT (north, security room) or SERVICE (south tunnel).
Do not let the creature touch you. Stand still to hide — it hunts by sound.

v6 — EXPANDED LAB + NEW SYSTEMS (2026-10-16)
-------------------------------------------
Map expanded 15x11 -> 19x14 (+65% explorable floor). New east wing holds the
SECURITY / CCTV room (monitor wall, operator desk, fallen guard, 2 audio logs)
and the VENT exit; new south wing holds the SERVICE exit and storage rooms.
Six new systems: (1) FLASHLIGHT (F) — warm spotlight, ~3 min battery,
recharges when off, battery-cell pickups; the specimen SEES the beam.
(2) SECURITY CAMERAS (C) — 5 fixed cams, live view of the specimen's current
position, phosphor-green static feed; the sim keeps running while you watch.
(3) SPEEDRUN TIMER — MM:SS.mmm from intro-exit to escape, best per difficulty
in localStorage, win screen shows time/best/NEW BEST/exit used. (4) ADRENALINE
(X) — 3 hidden syringes, 10s +40% speed, no stamina drain, 30s cooldown,
audible hiss. (5) AUDIO LOGS — 5 recovered recordings (E to play), amber
cassettes, LOGS n/5 counter + map intel. (6) THREE EXITS — MAIN/VENT/SERVICE
with distinct risk profiles. Key rebinding: F torch, E read, G radio, C cams,
X shot, Z crouch (was C).

ORIGINALITY NOTE
----------------
All game code was written from scratch for this jam. The only third-party
component is the Three.js r128 library (MIT licensed, bundled locally as
three.min.js). No network requests are made at any point.

v2 — ABANDONED LABORATORY ART PASS (2026-10-16)
----------------------------------------------
Per Tim's direction the facility now reads as a lab, not a dungeon: brushed-metal /
tiled walls with cyan conduit strips, 2.6 m dropped ceilings with dead and flickering
fluorescent troffers (patterned flicker, synced buzz), hazard striping, an empty
ajar containment chamber, lab benches with monitors (one flickering), scattered
papers, overturned stool, pipes and cable trays, "LAB 7" signage, biohazard decals,
and keycard readers (red->green) by the doors. The EXIT sign stays dark until 3/3
keycards, then lights green. The creature is now "the wrong human" (~2.2 m, hunched,
long arms, reverse-jointed legs) with AMBER eyes whose brightness tracks suspicion;
you rarely see more than its eyes until it takes you — then a 2 s jumpscare:
0.4 s of total silence and a frozen world, a procedurally-drawn horror face
filling your screen with a 4-layer synthesized scream, then a hard cut to
black. (And sometimes you hear a DISTANT scream that means nothing. Probably.)
Audio is fully positional (HRTF): the creature has a distinct voice per AI state,
the sonar ping's reverb tail changes between corridors and rooms, and the heartbeat
enters panic mode when it gets close. HUD is a phosphor-terminal lab instrument.
