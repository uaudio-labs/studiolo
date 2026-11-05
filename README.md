# StudioLo

A LUNA Add On that gives the open session a mixer styled after a late-80s cassette
portastudio: a cassette deck with turning reels and an LCD tape counter over a mixer with tape
scribble strips, colour-coded knobs and LED meters.

Requires LUNA 3.1.1 or later. The EQ and the Reverb and Delay buses use LUNA's built-in LUNA
Channel plug-in.

## Install

1. Download `studiolo.lunaaddon` from the latest release on this repository's **Releases**
   page.
2. Double-click the file. LUNA installs it into its Add Ons folder.

To update, install the newer `.lunaaddon` the same way.

## Use

Open it from **Add Ons > Apps > StudioLo**.

### Deck

- **+ Add track** adds an audio track (name it and choose Mono or Stereo), set up with LUNA
  Channel's four-band EQ and sends to Reverb and Delay buses, which it creates if
  the session has none.
- Click the cassette for the session selector: open a recent session, or create one. LUNA
  keeps one session open at a time, so this closes the current one.
- **Timeline** and **Mixer** switch LUNA's main window to that page.
- **Tempo** shows the BPM at the playhead. **+** and **−** change it by 1 BPM (0.1 with
  Shift); double-click to type a value.
- **Click** turns the metronome on and off. **RTZ** returns to zero. **Rec**, **Play/Pause**,
  **Stop** and **Loop** work as LUNA's own transport does, and follow it.

With no session open, only the cassette shows.

### Mixer

A strip for every visible track, then the buses, with the master last.

- Double-click a name to edit it (Enter saves, Escape cancels). Right-click a track's name for
  **Delete track**.
- **Fader:** drag to set the level; double-click resets to 0 dB. The dB scale matches LUNA's faders.
- **Pan:** drag up or right to turn; double-click centres; arrow keys nudge.
- **Meter** with a held peak and a clip light (click the light to clear it).
- **Mute** and **Solo**; audio and instrument tracks also have **REC** (record arm) and **MON**
  (input monitor).
- **Input** on audio tracks picks the track's input.
- **EQ:** four knobs (12 kHz, 2.5 kHz, 400 Hz, 60 Hz) for LUNA Channel's EQ in the channel's
  console slot. Without it they sit dimmed; click one to put LUNA Channel there (it replaces
  another console plugin).
- **Reverb** and **Delay** knobs set sends to the session's Reverb and Delay buses. Click a
  dimmed one to create the bus (if needed) and route the send.
- The **Reverb** and **Delay** buses have a **Settings** button under their name: it opens a
  panel to switch the effect on or off, pick its type (Plate, Hall, Cathedral, Digital, Spring;
  or Digital, Space Tape, Ping Pong) and turn its knobs (reverb mix, size, decay, pre-delay,
  damping, low and high cut, width, output; delay sync, time, feedback, mix). Click a value
  under a knob to type one ("3.5", "800 ms", "1k", "1/8T"); Enter sets it, Escape cancels.
- Click a strip to make it LUNA's focused and selected channel. The focused strip is lit, and
  follows focus changes made in LUNA.

Every drag is one undo step in LUNA.

### Timeline

Along the bottom, the whole session for one audio track: a bar ruler, the track's clips with
their waveforms, and the playhead. It shows the focused audio track.

- Click to move the play start, loop and edit selection there; drag to select a range.
- Drag the grip on its top edge to resize it; double-click the grip to reset.
