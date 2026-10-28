# Starting Something New

A hands-on learning log and project portfolio for building AI agents. I'm working through *AI Agents in Action, Second Edition* (Manning), running and modifying its examples, then building my own projects on top of what I learn.

The book's sample code lives in a separate repository (see [ATTRIBUTION.md](ATTRIBUTION.md)). Nothing here is a verbatim copy of it. Each learning-log folder holds my own notes and my modified versions of the examples.

## Goals

- Learn agent fundamentals by running and changing real code, not just reading.
- Build a small number of polished projects that solve real problems.
- Keep honest, clear credit for everything I adapt.

## Repository layout

| Path | What it is |
|---|---|
| `learning-log/` | One folder per book chapter: my notes, what I changed, what I learned |
| `projects/` | Standalone projects built from the ideas in the book (see the template in `projects/README.md`) |
| `ATTRIBUTION.md` | Source, license and credit conventions for adapted code |
| `THIRD_PARTY_LICENSES/` | License text of the upstream sample code |

## Progress

| Chapter | Topic | Status |
|---|---|---|
| 2 | First agents: model settings, structured output, tracing, tools | In progress |
| 3 | MCP servers and agents | Not started |
| 4 | Agent-to-agent workflows, handoffs, guardrails | Not started |
| 5 | Reasoning patterns (CoT, ReAct, and more) | Not started |
| 6 | Memory and retrieval | Not started |
| 7 | RAG grounding, image agents, tracing | Not started |

## Setup

Requires Python 3.11 or later. Node.js 20 or later is needed from chapter 3 onward, when MCP servers start.

```bash
python3 -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env            # then add your OPENAI_API_KEY
```

Run examples from the repository root:

```bash
python learning-log/chapter_02/01_first_agent.py
```

Never commit your `.env` file. It is listed in `.gitignore`.

## Attribution

The examples are based on the sample code for *AI Agents in Action, Second Edition* (Manning), published under the Apache License 2.0. See [ATTRIBUTION.md](ATTRIBUTION.md) for the source, the exact upstream version I started from, and how adapted files are marked.
