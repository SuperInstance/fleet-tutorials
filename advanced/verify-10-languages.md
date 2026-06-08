# Advanced Tutorial: Verify Mathematics Across 10 Languages
## What you'll prove
The same ternary→music mapping produces identical output in 10 different languages.
## Step 1: Clone the math foundations
```bash
git clone https://github.com/SuperInstance/fleet-math-foundations.git
```
## Step 2: Run each implementation
```bash
python3 implementations/python/bridge.py
cd implementations/rust && cargo test
node implementations/js/bridge.js
cd implementations/go && go run bridge.go
gcc implementations/c/ternary.c -o /tmp/t && /tmp/t
```
## Expected Output
All should show: Notes: [60, 64, 64, 60, 64, 64, 60, 64, 68]
