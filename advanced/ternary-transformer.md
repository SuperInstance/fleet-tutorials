# Advanced: Ternary Transformer Operations

Apply group operations to any ternary vector:

```python
from lib.transformer import TernaryTransformer
t = TernaryTransformer()
v = [1,0,-1,1,0,-1,1,1]

# Rotate (rhythmic shift)
rotated = t.rotate(v, 2)

# Invert (flip all values)
inverted = t.invert(v)

# Add (conservation applies)
sum_result = t.add(v, inverted)  # [0,0,0,0,0,0,0,0]

# Interpolate (morph between two states)
morphed = t.interpolate(v, [1,1,1,-1,-1,-1,1,1], 4)
```

The conservation law means v + invert(v) = [0...0] for any vector.
