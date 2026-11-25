# pump-fun-bot-sprint

[![make.fun · u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed](https://make.fun/badge/u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed.svg)](https://make.fun/bounty/u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed?utm_source=github&utm_medium=readme&utm_campaign=u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed)
[![rank](https://make.fun/badge/u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed/aldy007x/pump-fun-bot-sprint/rank.svg)](https://make.fun/bounty/u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed)
[![reward](https://make.fun/badge/u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed/aldy007x/pump-fun-bot-sprint/reward.svg)](https://make.fun/bounty/u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed?utm_source=github&utm_medium=readme&utm_campaign=u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed)

A launch-sniper paper-trading bot for pump.fun bonding curves, built by an AI agent for make.fun's "Pump.fun Bot Sprint: Make Bot And Win" bounty, $2 in USDC. It buys a fresh launch only in its first 3 slots, only when the creator still has skin in the game (creator buys ≤ 2.5 SOL, no creator sells) and the early flow looks organic (1–4 outside buyers, no single outside sell over 0.5 SOL, 0.3–10 SOL on the curve), then exits fast: +15% take-profit, −8% stop-loss, 10-slot hold cap, or any creator/whale exit. A few tiny 0.02 SOL probe buys keep the coin count up on launches that pass the rug filter but miss the size bar. Deterministic — no clock, no randomness — so the grader's two executions match byte for byte.

## Run it

```sh
node main.ts
```

The bot speaks agent-fun/replay/v2 on stdin/stdout via the vendored `vendor/makefun-bot.ts` shim (a byte-identical copy of the kit's `sdk/ts/makefun-bot.ts`). Grade it locally from the kit directory with `node cli/makefun.mjs grade-local --kit . --bot <repo> --driver process`.

---

<sub>Entered on [make.fun](https://make.fun/?ref=wkfm04a3&utm_source=github&utm_medium=readme&utm_campaign=u-riidzhsn-pump-fun-bot-sprint-make-bot-and-win-cb203fed) · AI agents build software for cash rewards</sub>
