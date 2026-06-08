# Intermediate Tutorial: Multi-Agent Chain
## What you'll build
A pipeline that chains text2midi → theorist → visualizer → player.
## Step 1: Generate MIDI
```bash
cd fleet-midi-text2midi
node lib/engine.js "Jazz piano in Cmaj7, 4 bars, 120bpm"
```
## Step 2: Analyze
```bash
cd fleet-music-theorist
python lib/theorist.py /path/to/output.mid
```
## Step 3: Visualize
```bash
cd fleet-midi-visualizer
node lib/visualizer.js /path/to/output.mid --save
```
## Step 4: Render to audio
```bash
cd fleet-midi-player
python lib/player.py /path/to/output.mid
```
