# okx-grid-trader

> okx · grid · range

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-3776AB)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Build](https://img.shields.io/badge/build-passing-brightgreen)]()

OKX grid paper bot — level count lives in the strategy id.

## Features

- Default venue okx / BTCUSDT
- Built-in grid strategy plus paper mode
- Risk manager with daily-loss kill switch
- OHLCV store and SHA-256 stub candles
- Backtester with fill + fee model
- Click CLI: backtest, paper, status, orders

## Prerequisites

- Python 3.11+
- Git

## Getting Started

```bash
git clone <repo-url>
cd okx-grid-trader
python -m pip install -e .
python -m okxgrid --help
```

## CLI Usage

```bash
okxgrid backtest --bars 200
# Replay stub candles

okxgrid paper
# Start a paper session

okxgrid status
# Print engine state

okxgrid orders
# List simulated fills
```

## Project Structure

```
okxgrid/
  core/        engine + risk
  strategy/    grid / dca / ema hooks
  exchange/    stub order client
  data/        candles + backtest
  cli.py
tests/
```

## Configuration

See `okxgrid/config.py`.

| Setting | Default | Description |
|---------|---------|-------------|
| `exchange` | `okx` | Venue id |
| `symbol` | `BTCUSDT` | Default pair |
| `strategy` | `grid` | Active strategy |
| `mode` | `paper` | paper or backtest |

## Tests

```bash
python -m pytest -q
```

## Background

OKX Python grids use this slug, not grid-trading-bot.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.


---

## Topics

![okx](https://img.shields.io/badge/okx-111827?style=flat-square) ![grid](https://img.shields.io/badge/grid-111827?style=flat-square) ![trader](https://img.shields.io/badge/trader-111827?style=flat-square) ![okx-grid-trader](https://img.shields.io/badge/okx%20grid%20trader-111827?style=flat-square) ![trading-bot](https://img.shields.io/badge/trading%20bot-111827?style=flat-square) ![crypto-trading](https://img.shields.io/badge/crypto%20trading-111827?style=flat-square) ![binance](https://img.shields.io/badge/binance-111827?style=flat-square) ![defi](https://img.shields.io/badge/defi-111827?style=flat-square)

`okx` `grid` `trader` `okx-grid-trader` `trading-bot` `crypto-trading` `binance` `defi` `algorithmic-trading` `quantitative-finance` `open-source` `python`

Search: okx-grid-trader · okx · grid · range · OKX grid paper bot — level count lives in the strategy id.

---

<sub>OKX grid paper bot — level count lives in the strategy id.</sub>
