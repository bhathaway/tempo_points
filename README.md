# Tempo Points

A practice tool for musicians that generates intermediate tempo markings between a start and end BPM using geometric progression — so each step increases by roughly the same ratio, matching how humans perceive tempo changes.

## Usage

Open `index.html` in any browser. Enter a start BPM, end BPM, and number of intermediate steps, then click **Generate** (or press Enter).

## How it works

Given start tempo **S**, end tempo **E**, and **N** intermediate points:

- Common ratio: `r = (E / S) ^ (1 / (N + 1))`
- Each tempo: `T_i = round(S * r^i)`

The average ratio is displayed as a percentage so you can judge whether your chosen number of steps is practical.

## Example

Start: 100 BPM, End: 200 BPM, Steps: 1

```
Avg ratio: ~41.4% per step

1. 100 bpm
2. 141 bpm
3. 200 bpm
```
