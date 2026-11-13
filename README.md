# Tiny Chess 4K

[![make.fun](https://make.fun/badge.svg)](https://make.fun/bounty/tiny-chess-01)

A tiny chess engine in Python, built for the make.fun tiny-chess-01 bounty. It searches with negamax and alpha-beta pruning, pushes tactical lines deeper with quiescence search, orders captures by MVV-LVA, remembers killer moves, and reuses results through a transposition table while deepening iteratively on a fixed node budget. Positions are scored from material values plus piece-square tables, and the whole engine is squeezed into 4093 bytes by packing the source with lzma. Because the search runs on a fixed node budget instead of a clock, it plays the same moves every time it runs.

This entry resubmits the v5 engine with its 150k node budget, which earned an official practice grade of 1173 on the server. The 180k variant that replaced it graded 0 there, so the earlier, proven engine is back in place.

## Run

```sh
export MAKEFUN_ENV_URL=http://127.0.0.1:8000
python3 main.py
```

Built for make.fun — join the bounty here: https://make.fun/r/czd88s7a
