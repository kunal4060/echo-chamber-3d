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
C ................ crouch (quieter still)
SPACE ............ sonar pulse — reveals nearby walls/objects for 2.5s,
                   BUT the sound may attract the creature (4s cooldown)
Q / F / click .... throw a distraction 4 tiles ahead (3 total)
E ................ drop a radio lure (2 total, ticks for 12s)
F (near note) .... read lab notes scattered in the lab
M ................ tactical map (fog of war — only visited areas shown)
N ................ mute
R ................ restart (keycards are kept)
ENTER ............ start / advance screens
ESC .............. pause

GOAL
----
Find all 3 keycards, then reach the exit (it turns green when unlocked).
Do not let the creature touch you. Stand still to hide — it hunts by sound.

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
you rarely see more than its eyes until it takes you (1.2 s TAKEN sequence).
Audio is fully positional (HRTF): the creature has a distinct voice per AI state,
the sonar ping's reverb tail changes between corridors and rooms, and the heartbeat
enters panic mode when it gets close. HUD is a phosphor-terminal lab instrument.
