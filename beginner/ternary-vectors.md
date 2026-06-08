# Beginner Tutorial: Understanding Ternary Vectors

## What they are

A ternary vector is just a list of three possible numbers:
- **+1** = go up (assertion, bright)
- **0** = stay (sustain, neutral)
- **-1** = go down (opposition, dark)

## Example

```
Vector: [1, 0, -1, 1, 0, -1, 1, 1]

+1 → go up a major third   (C → E)
 0 → stay on same note     (E → E)
-1 → go down a minor third (E → C)
+1 → go up again           (C → E)
 0 → stay                  (E → E)
-1 → go down               (E → C)
+1 → go up                 (C → E)
+1 → go up again           (E → G#)

Result: C E E C E E C E G#
```

## Why it matters

Any sequence of decisions can be a melody. Agent states, sensor readings,
game inputs — if you can represent it as -1, 0, +1, you can hear it.

## Next tutorial: [Browser Playback](browser-playback.md)
