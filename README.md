# Companion code: The Agentic AI Engineering Bible

Richard Boozman · Lincoln Publishers

## Contents

| Folder | What it holds |
|---|---|
| `agentlab/` | The companion library: model interface and scripted model, tools, agent loop, state, workflows, resilience, routing, RAG, memory, security, evaluations, multi-agent coordination, approvals and tracing |
| `examples/` | One script per chapter that has a listing (`chNN_*.py`) |
| `projects/m01_*` … `m12_*` | The twelve module projects, each with its own tests |
| `tests/` | Tests for the library |

## Quick start

```bash
python3 -m venv .venv && source .venv/bin/activate
pip install -e ".[all]"
python -m playwright install chromium     # only for Module VIII
python -m pytest                          # no API key needed: tests use scripted models
```

To run agents against a real model, set `AGENTLAB_PROVIDER` (`openai` or `anthropic`), `AGENTLAB_MODEL` and the provider's API key (see Appendix A). Never commit keys.

## What was tested

The examples and project tests were run on Python 3.13.16 on 22–23 October 2026: 120 tests passed.

These were not run:
- calls to live model providers (provider adapters were tested against a local fake server that follows the documented wire formats)
- Make scenarios
- the Module XI Docker image build

## Data

All companies, people, orders and invoices in the sample data are fictional.# Agentic-AI-Bible-companion-code
