# Event Cameras vs Frame Cameras

*Written: April 2026*

---

## My explanation

*[Write this in your own words after Day 1. Explain it like you're talking to a friend who hasn't heard of event cameras. This is the most important box to fill in.]*

---

## The analogy that helped me understand it

*[What mental model made this click for you?]*

---

## The key numbers worth remembering

| Property | Frame Camera | Event Camera |
|----------|-------------|--------------|
| Temporal resolution | ~33 ms (30 fps) | ~1 µs |
| Dynamic range | ~60 dB | >120 dB |
| Output | Full image every frame | (x, y, t, p) per brightness change |
| Power | High (all pixels always active) | Low (only changed pixels fire) |
| Motion blur | Yes | No |

*Source: Gallego et al. 2020*

---

## Why it matters for this project

*[How does this connect to the NanoLED hardware and the SNN software?]*

---

## What I still don't fully understand

*[Be honest. What would you struggle to explain to someone else?]*
