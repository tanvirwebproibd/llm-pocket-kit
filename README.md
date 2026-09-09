# llm-pocket-kit

Tiny streaming CLI for OpenAI-compatible chat APIs

Built for my own use; public in case it helps someone.

## Highlights

- Streams tokens as they arrive
- Reads the prompt from args or stdin
- Model and system prompt via flags or env
- Works with any OpenAI-compatible endpoint

## Installation

```bash
pip install -r requirements.txt
export OPENAI_API_KEY=sk-...
```

## Examples

```bash
chatsh explain this error < error.log
cat diff.patch | chatsh review this diff
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── chatsh.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT licensed, see LICENSE.
