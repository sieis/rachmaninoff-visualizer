# rachmaninoff-visualizer

A live piano visualizer for a connected MIDI instrument. One static file, no build.

**Live:** https://rachmaninoff-visualizer.netlify.app/

- Open `index.html` in Chrome or Edge (Web MIDI needs HTTPS or localhost), plug in a MIDI keyboard, play.
- `F` or double-click for fullscreen, `H` to toggle the controls.
- A sacred geometry backdrop turns behind the notes, colored from the same hue range as the keyboard. Pick a shape and set its complexity, spin, opacity, and saturation under Background in the controls.
- The backdrop listens to what you play. Each layer swells and brightens with its register, the hue drifts with the key you are in, and lines stitched between your notes build a kaleidoscope figure that fades after you let go. Play response (Background) sets how much, and 0 turns it off.
- Set Appears (Background) to When played and the backdrop has no existence of its own. Each note draws a few rings of the figure's own lines: its register picks the layer, bass at the rim and treble at the core, and its pitch picks which lines. They draw themselves in around the figure, shimmer while the key is held, then unravel and fade after the release.
- Rain or snow can fall behind the notes and splash on the top edge of the keyboard (Background, Weather).
- Deploys to Netlify as is.
