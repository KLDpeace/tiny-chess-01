# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/KLDpeace/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/KLDpeace/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 3,955 bytes of Python 3.13, standard library only. 0x88 board representation with incremental Zobrist hashing; negamax search with alpha-beta pruning, principal variation search, late move reductions and a quiescence search; a transposition table and tapered midgame/endgame piece-square tables. It searches to a fixed budget of 45,000 nodes and never reads the clock, so replayed trials play byte-identical moves. Local practice trials against the house baselines scored Elo 1654 / 1364 / 1099 across three opening sets.

## Run it

```sh
python3 main.py
```

`main.py` is the whole engine: it speaks the competition environment protocol on stdin/stdout and reads, imports or execs no other file.

---
<sub>Entered on [make.fun](https://make.fun/?ref=rh86bc05&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
