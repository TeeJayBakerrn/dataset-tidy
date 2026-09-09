# dataset-tidy

Clean and split JSONL datasets for fine-tuning

## Install

```bash
# stdlib only
```

## Examples

```bash
python prep.py raw.jsonl --out-dir data/ --valid-ratio 0.1
```

## Features

- Length filters keep the sweet spot
- Deterministic split with a seed
- Prints a stats summary you can eyeball
- Dedup by normalized instruction text

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
└── prep.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
