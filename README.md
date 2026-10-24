<!-- Profile README: https://github.com/HarshithhKumar -->

<div align="center">

# Sampangi Harshith Kumar

**Computer Science Engineering · Backend Development · Applied Machine Learning**

Building practical software across APIs, full-stack applications, and sensor-based ML systems.

[GitHub](https://github.com/HarshithhKumar) · [LinkedIn](https://linkedin.com/in/sampangi-harish-kumar) · [Email](mailto:harshithkumar2023@gmail.com) · [LeetCode](https://leetcode.com/u/codewharshith/)

[![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)](https://isocpp.org/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)](https://react.dev/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![scikit--learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)

</div>

---

## About

I’m a Computer Science Engineering student at **SRM University AP** interested in backend systems, reliable APIs, and applied machine learning. I like connecting the pieces of a project—from data and persistence to model evaluation and the interface—and making the result understandable for another developer.

My work includes webhook automation, smartphone-sensor activity recognition, embedded interaction prototypes, and small ML pipelines. I’m also exploring the **Internet of Musical Things (IoMusT)** and connected interactive systems.

**Currently improving:** data structures and algorithms, backend reliability, database design, automated testing, and practical system design.

## Featured projects

<details>
<summary><strong>HookRelay</strong> — Reliable webhook processing and comment-to-DM automation</summary>

**FastAPI · PostgreSQL · SQLAlchemy · React · Docker**

A backend workflow that verifies incoming events, persists them, matches configured rules, and creates durable jobs for downstream message processing.

- Handles duplicate events, idempotency, retries/backoff, rate limits, and delivery-state reconciliation.
- Includes a React dashboard and a PseudoGram mock API for testing without claiming a live Instagram integration.
- Worker loops currently run inside the FastAPI process; a separate production worker deployment remains a future improvement.

**Focus:** API design, database modeling, and failure-aware asynchronous workflows.

[View repository](https://github.com/HarshithhKumar/HookRelay)

</details>

<details>
<summary><strong>Kinetix</strong> — Human activity recognition from motion sensors</summary>

**Python · TensorFlow/Keras · scikit-learn · FastAPI · React**

A full-stack classifier for six activities using accelerometer and gyroscope windows from the UCI Human Activity Recognition dataset. A Bidirectional LSTM model uses training-fitted scaling and serves predictions through FastAPI.

- **Reported test results:** 86.90% accuracy and 87.15% macro F1 on the UCI test set.
- The dashboard displays predictions, class probabilities, sensor traces, and evaluation information.
- Browser-based live-phone capture is experimental and has not been quantitatively evaluated.

**Focus:** time-series preprocessing, model evaluation, and ML/API/frontend integration.

[View repository](https://github.com/HarshithhKumar/Kinetix)

</details>

<details>
<summary><strong>GestureFusion</strong> — Embedded sensing and gesture-interaction prototype</summary>

**ESP32 · MATLAB · Python · scikit-learn · Signal Processing**

An exploration of a sensor-to-classifier workflow, connecting embedded motion sensing with signal processing, feature extraction, and model training.

- Includes a lightweight Random Forest training workflow and saved model/metrics artifacts.
- The current pipeline uses **synthetic data**, so its metrics validate the workflow rather than real-world gesture accuracy.
- The next step is evaluation on genuine sensor recordings.

**Focus:** embedded/ML integration and cross-disciplinary prototyping.

[View repository](https://github.com/HarshithhKumar/GestureFusion)

</details>

<details>
<summary><strong>Burnly</strong> — Calorie-estimation regression demo</summary>

**Python · scikit-learn · pandas · NumPy · pytest**

A small tabular regression workflow covering data preparation, model training, saved artifacts, evaluation output, and visual exploration.

- The current workflow can use synthetic data; results should not be treated as real-world or clinical accuracy.
- A documented real dataset and leakage-safe evaluation would be needed for a meaningful performance assessment.

**Focus:** reproducible ML pipelines and regression evaluation.

[View repository](https://github.com/HarshithhKumar/Burnly)

</details>

## Technical toolkit

| Area | Tools and concepts |
|---|---|
| **Languages** | C++, Python, JavaScript, SQL |
| **Backend** | FastAPI, REST APIs, Pydantic, Uvicorn, SQLAlchemy |
| **Frontend** | React, Vite, Axios, HTML, CSS |
| **Data and storage** | PostgreSQL, relational modeling, migrations, durable job state |
| **Machine learning** | TensorFlow, Keras, scikit-learn, NumPy, pandas, time-series classification, regression, model evaluation |
| **Embedded and signals** | ESP32, Arduino, MATLAB, Simulink, accelerometer/gyroscope data, MIDI, OSC/UDP |
| **Engineering tools** | pytest, Git, GitHub Actions, Docker, Linux |

## Current focus

- **Problem solving:** Practice DSA and complexity analysis in C++ and Python.
- **Backend reliability:** Improve validation, transactions, retries, idempotency, and error handling.
- **System design:** Learn schema design, indexing, caching, and service boundaries.
- **Testing and CI:** Add meaningful unit/integration tests and reproducible automated checks.
- **Applied ML:** Strengthen baseline comparisons, leakage prevention, and class-level evaluation.

---

<div align="center">

**Open to software engineering and backend development opportunities.**

</div>
