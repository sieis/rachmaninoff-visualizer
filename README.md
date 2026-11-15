# rachmaninoff-visualizer

A live piano visualizer for a connected MIDI instrument. One static file, no build.

**Live:** https://rachmaninoff-visualizer.netlify.app/

- Open `index.html` in Chrome or Edge (Web MIDI needs HTTPS or localhost), plug in a MIDI keyboard, play.
- `F` or double-click for fullscreen, `H` to toggle the controls.
- A sacred geometry backdrop turns behind the notes, colored from the same hue range as the keyboard. Pick one of thirteen shapes under Geometry in the controls and set its complexity, size, line weight, spin (either direction), opacity, and saturation.
- The backdrop listens to what you play. Each layer swells and brightens with its register, the hue drifts with the key you are in, and lines stitched between your notes build a kaleidoscope figure that fades after you let go. Play response (Reaction) sets how much, and 0 turns it off.
- Set Geometry appears (Reaction) to When played and the backdrop has no existence of its own. Each note draws a few rings of the figure's own lines: its register picks the layer, bass at the rim and treble at the core, and its pitch picks which lines. They draw themselves in around the figure, shimmer while the key is held, then unravel and fade after the release. Draw speed and Fade time, shown while this mode is on, set how fast the lines draw in and how long they linger.
- Among the shapes: Circle of fifths joins the notes you hold into the shape of their chord, and Platonic solids turn in three dimensions.
- Three buttons at the top of Keyboard pick what a note sends up the screen. Off sends nothing: the keys light up in the note's color and glow, and only Glow, Hue, Color spread, and Keyboard height remain. Note visualizer is the rising bars with every option. Wireframe turns the backdrop grey and fires a wire from each key to a random point on its rim; where the wire lands, the note's color runs into the figure in threads along its own lines for as long as the key is held. Even a short note spreads far: Spread time (Reaction) sets how long the color keeps running after the wire lands, before it starts to fade. Draw speed and Fade time set how fast the threads run and how long the fade takes.
- Color by (Keyboard) picks what sets a note's color: its place on the keyboard, its pitch class so octaves match, or how hard it was struck. Velocity sensitivity sets how much a hard strike brightens and widens its bar.
- Particles have their own section: amount, speed, spread, size, and lifetime.
- Rain or snow can fall behind the notes and splash on the top edge of the keyboard (Weather). Wind leans it either way and Fall speed sets its pace.
- Upload a picture to sit behind everything (Image), then set its opacity, blur, and dim. It stays in your browser and is not part of a preset.
- Deploys to Netlify as is.
