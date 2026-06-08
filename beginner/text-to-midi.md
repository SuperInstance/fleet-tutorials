# Beginner Tutorial: Text to MIDI

## What you'll do
Type a sentence. Get a MIDI file. Your first encounter with the fleet.

## Step 1: Install

```bash
git clone https://github.com/SuperInstance/fleet-midi-text2midi.git
cd fleet-midi-text2midi
npm install
```

## Step 2: Generate

```bash
node lib/engine.js "C major chord"
```

You'll see output like:
```
✅ MIDI generated: /path/to/output.mid
```

## Step 3: What happened

The text "C major chord" was parsed by music21 (music theory library).
It understood: key=C, major quality, chord = C-E-G triad.
It generated a MIDI file with those three notes.

## Next tutorial: [Ternary Vectors](ternary-vectors.md)
