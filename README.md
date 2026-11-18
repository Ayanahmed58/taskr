# taskr

[![CI](https://github.com/YOUR-USERNAME/taskr/actions/workflows/ci.yml/badge.svg)](https://github.com/YOUR-USERNAME/taskr/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![Python](https://img.shields.io/badge/python-3.9%2B-blue)

A tiny, dependency-free to-do manager for your terminal. Tasks live in a single JSON file you can back up, sync, or edit by hand.

## Features

- Zero runtime dependencies
- Simple commands: `add`, `list`, `done`, `rm`
- Plain JSON storage (`~/.taskr.json`, or set `TASKR_FILE`)
- Fully tested, with CI on Python 3.9 to 3.13

## Installation

```bash
git clone https://github.com/YOUR-USERNAME/taskr.git
cd taskr
pip install .
```

## Usage

```console
$ taskr add Buy groceries
Added #1: Buy groceries
$ taskr add Write README
Added #2: Write README
$ taskr done 1
Completed #1: Buy groceries
$ taskr list
[x] 1. Buy groceries
[ ] 2. Write README
$ taskr list --pending
[ ] 2. Write README
$ taskr rm 2
Removed #2
```

## Development

```bash
pip install -e ".[dev]"
pytest
ruff check .
```

## Roadmap

- [ ] Due dates and priorities
- [ ] Tags and search
- [ ] Export to Markdown

## Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[MIT](LICENSE)
