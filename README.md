# Vibe-coded BattleCity

launch:

prompt:

Build a third person view adventure shooter game as a single self-contained index.html. See AGENTS.md
for the Kenney asset pipeline — follow it exactly.

Tech: Three.js r160 via importmap (no build step, no npm). Runs with
`python3 -m http.server 8080`

Player: a mini character from the Kenney mini-characters pack. 3 selectable
variants (use the rest as NPC enemies). continuous movement with animation.

Assets: load the REAL Kenney GLB models — first list the three GLB folders
(kenney_mini-characters, kenney_blaster-kit, kenney_city-kit-industrial_2.0, each under
`assets/<pack>/Models/GLB format/`) to get exact filenames, then load/cache/clone them
(see AGENTS.md). Use a colored box only as a per-file fallback, not the default.

World: infinite city built with kenney city kit
randomly distribute supply boxes that can be opened for new weapons or health or ammunition


Feel: isometric follow camera with smooth lerp; WebAudio SFX for weapons firing
weapon hits and supply pickups; particle bursts; camera shake on damage; button to switch weapons.

UI: time survived and enemies killed
with restart; high score in localStorage.

Acceptance criteria:
- left click  moves the character  with smooth animation.
- right click fires the character weapon.
small circular red reticle that tracks the mouse shows where the player is aiming.

- Runs via python3 -m http.server, single index.html, no build step.

Build the complete game now
