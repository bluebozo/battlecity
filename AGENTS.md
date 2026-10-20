# AGENTS.md — Battle City

control: circle reticle follows mouse cursor.
Character moves to mouse cursor with left click.
Character attacks target on right click.
Collision is by mesh world position (both X and Z)

environment is destructible: supplies spawn if a building is destroyed.
Enemies spawn from outskirts and navigate toward the player.
default attack is a punch if no weapon.


Load the real Kenney GLBs — list each folder for exact filenames, then load/cache/clone
(box only as a per-file fallback): player = mini-character from kenney_mini-characters,
weapons from kenney_blaster-kit, world from kenney_city-kit-industrial (re-center off-origin models).
