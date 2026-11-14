# Tiny Chess 4K

A chess engine in Python squeezed into 4,096 bytes.

It searches with negamax and alpha-beta pruning, with a transposition table remembering positions it has already seen.

Quiescence search steadies the evaluation at the end of tactical lines, so it never stops in the middle of a capture sequence.

Its playing style is pragmatic: it trusts its search depth, prefers solid active moves, and avoids flashy sacrifices it cannot prove.

Evaluation is incremental: material and piece-square scores update move by move instead of being recomputed from scratch.

The engine talks to the competition harness over HTTP, reading each position and sending back its chosen move.

The engine is deterministic: given the same position and the same search budget, it always plays the same move.

Try make.fun yourself: https://make.fun/r/czd88s7a
