<!-- Profile README: https://github.com/HarshithhKumar -->

<div align="center">

# Sampangi Harshith Kumar

**Computer Science Engineering | Software Development | Applied Machine Learning**

I design and build software across backend services, full-stack applications, machine-learning pipelines, and embedded systems. I enjoy understanding how a system works end to end—from data collection and API design to persistence, evaluation, and the user interface.

[GitHub](https://github.com/HarshithhKumar) · [LinkedIn](https://linkedin.com/in/sampangi-harshith-kumar) · [Email](mailto:harshithkumar2023@gmail.com) · [LeetCode](https://leetcode.com/u/codewharshith/)

</div>

---

## Profile

I am a Computer Science Engineering student at **SRM University AP** with interests in backend engineering, reliable APIs, applied machine learning, and connected interactive systems. My projects span event-driven backend workflows, sensor-based activity recognition, embedded interaction prototypes, and model-training pipelines.

My approach is to make projects understandable and reproducible: explain the architecture, document how to run the code, test the important paths, and distinguish measured results from experimental features.

- **Research:** Internet of Musical Things (IoMusT), exploring connected musical and interactive systems.
- **Engineering interests:** Backend services, API design, database-backed workflows, full-stack development, and software quality.
- **Machine learning interests:** Time-series classification, data preprocessing, model evaluation, and reproducible experiments.
- **Currently developing:** Data structures and algorithms, system-design fundamentals, automated testing, and production-oriented engineering practices.

## Featured projects

### 1. [HookRelay](https://github.com/HarshithhKumar/HookRelay)
**Reliable webhook processing and comment-to-DM automation**  
*FastAPI · PostgreSQL · SQLAlchemy · React · Vite · Docker*

HookRelay models the path from an incoming social-media comment event to a reliable outbound direct-message job. Instead of treating a webhook as a one-off HTTP request, the application verifies the incoming event, persists it, matches it against configured rules, and creates a durable job for downstream processing.

The core engineering focus is reliability under imperfect conditions. Webhooks can be delivered more than once, upstream APIs can fail temporarily, rate limits can be reached, and an accepted message may not yet be confirmed as delivered. HookRelay addresses these cases with event deduplication, database-backed job state, stable idempotency keys, retry/backoff handling, rate limiting, and delivery reconciliation. Its data model records events, jobs, send attempts, and delivery state so the application can reason about work after failures or restarts.

The project includes a FastAPI backend, PostgreSQL persistence and migrations, a React dashboard, and a PseudoGram mock upstream API for exercising the messaging workflow without claiming a live Instagram integration. Worker loops currently run inside the FastAPI process, a documented simplification rather than a separate production worker deployment.

**Engineering highlights**
- Verify signed webhook requests before processing event data.
- Persist and deduplicate events to protect against repeated deliveries.
- Create durable jobs with stable idempotency keys and explicit retry state.
- Handle rate limiting and reconcile accepted messages with final delivery status.
- Expose API health and operational statistics through a dashboard.

**What it demonstrates:** API design, database modeling, idempotent processing, failure handling, and the trade-offs involved in building dependable asynchronous workflows.

### 2. [Kinetix](https://github.com/HarshithhKumar/Kinetix)
**Human activity recognition from smartphone motion sensors**  
*Python · TensorFlow/Keras · scikit-learn · FastAPI · React · Vite*

Kinetix is a full-stack machine-learning application that classifies motion into six activities: walking, walking upstairs, walking downstairs, sitting, standing, and laying. It uses the UCI Human Activity Recognition Using Smartphones dataset, which contains accelerometer and gyroscope measurements collected in fixed-length time windows.

The model pipeline accepts a window of 128 time steps and six inertial features. A training-fitted StandardScaler normalizes the sensor values before they enter a Bidirectional LSTM-based classifier. The saved model is served through a FastAPI inference API, while a React dashboard lets users inspect predictions, class probabilities, sensor traces, and evaluation information.

The repository reports **86.90% test accuracy** and **87.15% macro F1** on the UCI test set. These are dataset evaluation results, not a claim that the model has been validated across arbitrary devices or real-world environments. The browser-based live-phone mode is experimental and has not been quantitatively evaluated.

**Engineering and ML highlights**
- Work with sequential, multivariate time-series sensor data.
- Keep scaling consistent between training and inference and fit preprocessing on training data.
- Serve model predictions through a documented API.
- Compare predicted activity with ground truth and inspect class-level results.
- Separate the reproducible dataset demo from experimental browser sensor capture.

**What it demonstrates:** ML inference integration, time-series preprocessing, model evaluation, API/frontend integration, and communicating limitations honestly.

### 3. [GestureFusion](https://github.com/HarshithhKumar/GestureFusion)
**Embedded sensing and gesture-interaction prototype**  
*ESP32 · MATLAB · Python · scikit-learn · Signal Processing*

GestureFusion explores a pipeline that connects motion sensing, signal processing, and software-based gesture classification. Its intended system spans ESP32-based sensor collection, MATLAB processing and feature-extraction materials, and Python tools for training and visualizing a classifier.

The repository provides a lightweight training workflow that generates a synthetic dataset, splits it into training and test subsets, trains a Random Forest classifier, and saves a model artifact alongside a metrics report. This makes it possible to exercise the model-training and artifact-generation workflow without needing a complete real-world gesture dataset.

An important limitation is that the current training pipeline uses **synthetic data**. Its metrics therefore test the workflow, not real-world gesture-recognition performance. The project is a foundation for integrating genuine sensor recordings, documented features, and a more meaningful evaluation protocol.

**Engineering highlights**
- Connect embedded sensing concepts with downstream software processing.
- Organize MATLAB and Python components around a wider interaction prototype.
- Generate repeatable training inputs and save model and evaluation artifacts.
- Provide a dashboard and notebook materials for exploration.

**What it demonstrates:** cross-disciplinary prototyping, data-pipeline organization, embedded/ML integration concepts, and a clear path from a demo toward evaluation on real sensor data.

### 4. [Burnly](https://github.com/HarshithhKumar/Burnly)
**Tabular regression and model-evaluation workflow**  
*Python · scikit-learn · pandas · NumPy · pytest*

Burnly explores a supervised regression workflow for estimating calorie expenditure from physiological and activity-related features. The repository organizes dataset loading, preprocessing, model training, saved artifacts, evaluation output, and visual exploration into a small project that can be run and inspected.

The current workflow can use synthetic data, so its reported metrics should not be interpreted as evidence of real-world or clinical accuracy. A meaningful next step is to evaluate the model on a suitable documented real dataset, define a leakage-safe train/test protocol, and compare the baseline against appropriate alternatives.

**Engineering highlights**
- Structure a tabular ML workflow from input data to saved model.
- Export evaluation metrics and visual artifacts for inspection.
- Include tests and a notebook/dashboard for exploring the pipeline.

**What it demonstrates:** practical ML workflow organization, regression evaluation, artifact management, and reproducibility. It is an educational project, not a clinically validated calorie estimator.

---

## Technical toolkit

**Programming languages**  
C++, Python, JavaScript, SQL

**Backend and APIs**  
FastAPI, REST API design, Pydantic, Uvicorn, SQLAlchemy

**Frontend development**  
React, Vite, Axios, HTML, CSS, JavaScript

**Databases and persistence**  
PostgreSQL, relational data modeling, database migrations, durable job state

**Machine learning and data science**  
TensorFlow, Keras, scikit-learn, NumPy, pandas, time-series preprocessing, classification, regression, model evaluation

**Embedded systems and signal processing**  
ESP32, Arduino, MATLAB, Simulink, accelerometer/gyroscope data, MIDI, OSC/UDP

**Testing and developer tooling**  
pytest, Git, GitHub, GitHub Actions, Docker, Linux, automated build and test workflows

## Current focus

- **Data structures and algorithms:** Improve problem-solving fluency, complexity analysis, and implementation quality in C++ and Python.
- **Backend engineering:** Build APIs with clear validation, predictable error handling, database transactions, and maintainable service boundaries.
- **Reliability and asynchronous workflows:** Deepen understanding of idempotency, retries, rate limits, durable queues, observability, and recovery from partial failure.
- **Databases and system design:** Practice schema design, indexing, consistency trade-offs, caching, and designing components that can evolve as requirements grow.
- **Testing and CI:** Expand unit and integration coverage, make test environments reproducible, and use automated checks to catch regressions before merging.
- **Applied machine learning:** Strengthen preprocessing discipline, baseline comparisons, leakage prevention, class-level evaluation, and reproducible experiments.
- **Project documentation:** Make every featured repository easier to set up, understand, test, and evaluate through architecture notes, realistic examples, and clearly stated limitations.

## Engineering principles

I aim to build software that is understandable, testable, and honest about its capabilities. I value clear architecture over unnecessary complexity, reproducible evaluation over unsupported performance claims, and documentation that helps another developer run the project and understand its trade-offs.

---

<div align="center">

**Open to software engineering and backend development opportunities.**

</div>
