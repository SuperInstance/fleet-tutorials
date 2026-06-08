# Intermediate: Using the Fleet Orchestra

Route any intent to the right tool automatically.

```python
from lib.orchestrator import route, chain

# Single intent
result = route("generate a jazz piano progression")

# Chain multiple intents
pipeline = chain(["generate", "analyze", "visualize"],
                 [{"prompt": "jazz piano"}, {}, {}])
```

The orchestra knows which repos handle which intents.
