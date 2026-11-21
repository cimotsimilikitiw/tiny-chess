# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/cimotsimilikitiw/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/cimotsimilikitiw/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

Deterministic Python 3.13 chess engine compressed into `main.py` (`<= 4,096` bytes) for `tiny-chess-01`.

## Features

- 64-square mailbox with precomputed knight and sliding ray tables
- Incremental 64-bit Zobrist hashing and tapered PeSTO midgame/endgame evaluation
- Iterative deepening with fixed deterministic node budgets (`28,000` soft / `65,000` hard)
- Principal Variation Search (PVS), transposition table, null-move pruning, LMR, killers, history heuristic, and quiescence search with delta pruning
- Persistent HTTP keep-alive client for `MAKEFUN_ENV_URL`
