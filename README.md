# Evolutionary Racing AI

A small 2D racing simulation for studying one question:

> Does initialising PPO from a genetically-evolved policy improve learning
> efficiency, final performance or robustness compared with PPO trained from scratch?

Three methods are compared under the same environment, interaction budget and
evaluation protocol: **GA**, **PPO**, and **GA -> PPO**. The hybrid is a hypothesis
to test, not an assumed winner.

## Status

Early development. Currently building the environment (see roadmap below).

## Roadmap

- [x] Project scaffold and CI
- [ ] Track format and the six core tracks
- [ ] Vehicle, sensors, checkpoints, reward components
- [ ] Rule-based baseline controller
- [ ] Genetic algorithm
- [ ] PPO baseline
- [ ] GA -> PPO transfer with critic warm-up
- [ ] Controlled experiments and analysis

## Setup

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt -r requirements-dev.txt
pip install -e .
pytest
```

## Design decisions

_Added as the project develops._
