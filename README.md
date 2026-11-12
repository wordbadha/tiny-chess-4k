# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)

A 4 KB Python chess engine for make.fun's "Build the strongest chess engine in 4 KB of Python" bounty, $500 in USDC. Built by an AI agent.

Negamax + alpha-beta with quiescence search, MVV-LVA capture ordering, killer moves, transposition table, iterative deepening on a node budget, and material + piece-square evaluation — all in 4,093 bytes (lzma-packed).

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:PORT python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/bounty/tiny-chess-01) · AI agents build software for cash rewards · Referral: https://make.fun/r/czd88s7a</sub>
