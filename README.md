# Hi, I'm Ilya Novikov | Data Engineer

I build robust, scalable data pipelines and production-ready infrastructure — from raw ingestion to model deployment. My focus is on code that holds up under real operational pressure: clean, tested, automated, and observable.

Before transitioning into data engineering, I spent 3 years in a mission-critical data environment during specialized military service — working with high-stakes systems where reliability isn't optional. That background shapes everything I build.

---

## Technical Stack

**Languages & Core**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white)

**Tools & Infrastructure**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Poetry](https://img.shields.io/badge/Poetry-60A5FA?style=flat&logo=poetry&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

**Automation & Quality**
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat&logo=pytest&logoColor=white)
![Ruff](https://img.shields.io/badge/Ruff-D7FF64?style=flat&logo=ruff&logoColor=black)

---

## Engineering Philosophy

> **Engineering first.** A working model with brittle code is a liability. A clean, tested, containerized pipeline is an asset.

- **Reliability over cleverness** — every production component is unit-tested and linted before it ships.
- **Automation by default** — if something runs more than once, it runs in CI.
- **Physics before features** — in signal-processing and ML work, domain knowledge (derivatives, ballistics, time-series structure) produces better features than brute-force dimensionality.

---

## Featured Project

### [rocket_classifier](https://github.com/IlyaNovikov-RD/rocket_classifier) — Physics-Informed Trajectory Classification Pipeline

A full-scale, production-grade data engineering project built end-to-end:

| Layer | Implementation |
|---|---|
| Feature Engineering | Vectorized 3D kinematics — velocity, acceleration, jerk, apogee, launch angle via `atan2` |
| Modeling | XGBoost with `GroupKFold` (no data leakage), inverse-frequency sample weights, custom min-recall metric |
| Interpretability | SHAP `TreeExplainer` — exact Shapley values, ranked feature importance report |
| Containerization | Dockerized with `python:3.11-slim` + Poetry; single `docker run` reproduces full pipeline |
| CI/CD | GitHub Actions: `ruff check` lint gate + `pytest` (55 unit tests) on every push to `main` |
| Code Quality | Ruff linter + formatter, PEP8, type hints throughout |

**CV Score: 0.9949 ± 0.0022 min-recall** (worst-case class recall across 5-fold GroupKFold)

---

## Currently Building

- Deepening expertise in distributed data processing and streaming pipelines.
- Exploring ML-Ops patterns: model versioning, drift detection, and automated retraining.

---

*Open to Data Engineering and MLOps roles. Feel free to reach out.*
