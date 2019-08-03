# godot-randomsound
RandomSound is a custom node which can play from a random AudioStreamPlayer and apply override modifiers to pitch and volume in addition to supporting multiple channels.  It is intended as a mostly-compatible drop-in replacement for AudioStreamPlayer in places where one from a pool of random sounds is needed.


# Usage
Recommended usage is to instance a scene from RandomSound.tscn.  It registers itself as a class, but may not automatically create the appropriate "Channels" node to store channels for playback if instanced from the New Node dialog.  Place your AudioStreamPlayers into the root of RandomSound.  **Do NOT place nodes in `Channels` as these are subject to be dynamically reallocated when the number of channels changes.**

# Features planned...?
	* AudioStreamPlayer2D / 3D
	* Playing all children in an AudioStreamPlayer together
	* Nested `RandomSound`s
	