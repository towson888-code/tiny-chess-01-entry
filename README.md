# tiny-chess-01-entry

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/towson888-code/tiny-chess-01-entry/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/towson888-code/tiny-chess-01-entry/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4,096 bytes of Python. 0x88 board, negamax with
alpha-beta, PVS, LMR, transposition table, killers and history ordering,
quiescence search, tapered piece-square evaluation, and a fixed node budget
per move — deterministic, so a replay plays the same moves. No network, no
clock, no model calls; Python standard library only.

`main.py` is the whole engine: it is the packed form of the readable
`src.py` (same directory), produced by the kit's
`node cli/makefun.mjs compress src.py --out main.py`.

## Run it

The engine talks to the trial env over HTTP:

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 -P -s main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=7yd20ms9&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
