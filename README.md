# Predicting Value and Ranking Social Volatility of Cryptocurrency via Twitter

[![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

> The Dream Team's... dream!

A group project for an undergraduate Advanced Data Analytics course that aims to
analyze the relationship between tweets and cryptocurrencies.

## Install

### Built With

- [The CryptoCompare API](https://min-api.cryptocompare.com/)
- [cryptocompare](https://github.com/lagerfeuer/cryptocompare#readme)
- [Tywthon](https://github.com/ryanmcgrath/twython#readme)

### Prerequisites

- [uv](https://docs.astral.sh/uv/getting-started/installation/)

### Setting up Development Environment

```console
git clone https://github.com/bryan-hoang/cmpe-351-group-project.git
cd cmpe-351-group-project/
uv sync
```

`uv sync` creates a virtual environment and installs all dependencies related to
the project and for development. To activate the virtual environment, run
`source .venv/bin/activate`.

### Configuration

For security, the code retrieves the secrets of API keys needed for building the
dataset from environment variables. For convenience, the project uses `.env`
files to store these secrets.

You will need to create a `.env` file at the root of the project and set the
`CRYPTOCOMPARE_API_KEY`, `TWITTER_APP_KEY`, and `TWITTER_APP_SECRET` environment
variables if you want to run
[src/1_get_raw_dataset.ipynb](src/1_get_raw_dataset.ipynb). e.g.,

```txt
# .env
CRYPTOCOMPARE_API_KEY='YOUR_CRYPTOCOMPARE_API_KEY'
TWITTER_APP_KEY='YOUR_TWITTER_APP_KEY'
TWITTER_APP_SECRET='YOUR_TWITTER_APP_SECRET'
```

## Usage

For example,

```console
uv run python src/3_exploratory_visualization.py
```

## Maintainers

- [@bryan-hoang](https://github.com/bryan-hoang)
- [@leighddrr](https://github.com/leighddrr)
- [@16ymf1](https://github.com/16ymf1)
- [@james-zhu2000](https://github.com/james-zhu2000)

## Contributing

Small note: If editing the README, please conform to the
[standard-readme](https://github.com/RichardLitt/standard-readme) specification.

## License

MIT © 2022 Bryan Hoang and contributors
