# tiny-chess-01 — fresh rebuild

A chess engine in 4,096 bytes of Python (main.py, 3,622 bytes).
Negamax + alpha-beta + quiescence, fixed depth 3, deterministic
(no clock, no randomness). Evaluation: material + piece-square
tables. Talks to the env at MAKEFUN_ENV_URL (POST /game, POST /move).

Rebuilt from scratch after the first entry was rejected by the server
(thinking_priced). Verified: perft(3) = 8,902 from the start position,
finds mate-in-1 (Qxf7#), ~0.05 s a move in the opening.

License: MIT.
