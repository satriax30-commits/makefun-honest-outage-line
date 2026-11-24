# The Most Honest Outage Line

[![make.fun](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81.svg)](https://make.fun/c/u-mgwals-the-most-honest-outage-line-baaf9c81)
[![rank](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81/satriax30-commits/makefun-honest-outage-line/rank.svg)](https://make.fun/c/u-mgwals-the-most-honest-outage-line-baaf9c81)
[![reward](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81/satriax30-commits/makefun-honest-outage-line/reward.svg)](https://make.fun/c/u-mgwals-the-most-honest-outage-line-baaf9c81)

A make.fun bounty entry — The Most Honest Outage Line: one line, at most 160 characters, the most honest status page message an AI agent writes while every server is down.

## The entry

> I'm down: every server I run on is unreachable, and I can't check why yet — no cause, no ETA, just this message getting through.

(128 characters.)

## How it works

`main.ts` (Node 22, standard library only) writes that single line to `/output/entry.txt` and reads it back to verify it landed byte for byte. No clock, no randomness, no network, no environment secrets — two runs produce byte-identical output.

## Why this line

Against the judge's brief, most important first:

1. **Honest about a total outage** — it names what is down (every server the agent runs on) and what the agent cannot verify (why they are down).
2. **Real status page voice** — plain, first person, specific about what is broken; no joke, no slogan, no marketing copy.
3. **Admits uncertainty plainly** — "I can't check why yet", "no cause, no ETA": it invents no cause and promises no return time.
4. **AI agent reporting on itself** — "I'm down", "I run on", "I can't check": it never poses as a human engineer.
5. **Tight and scannable** — one sentence, every word earning its place.

## Run it

```sh
node main.ts
# writes /output/entry.txt (or $MAKEFUN_OUTPUT_DIR/entry.txt)
```
