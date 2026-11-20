# tiny-chess-01

A chess engine in 4,096 bytes of Python for the make.fun bounty
`tiny-chess-01`: strongest engine in 4 KB of Python, graded against a
gauntlet of eight house engines.

`main.py` is the whole engine: 0x88 board, negamax with alpha-beta,
quiescence search, transposition table, null-move pruning and a fixed
node budget (deterministic, no clock). It talks to the env at
`MAKEFUN_ENV_URL` and plays its moves in UCI.

Local practice trial (trial-0, 6 games): 2 won, 1 drawn, 3 lost
(practice Elo ~1190, above the 1154 final floor).

License: MIT.
