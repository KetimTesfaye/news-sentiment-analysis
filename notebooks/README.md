Financial News Sentiment Analysis

Project Overview
This project aims to analyze a large-scale financial news dataset to extract actionable insights and correlate news sentiment with stock market movements. This repository follows professional data engineering standards, including modular directory structures and automated CI/CD pipelines.

Task 1: Exploratory Data Analysis (EDA) & Infrastructure

 1. Environment & Infrastructure
- Branching: All development for Task 1 was conducted on the `task-1` branch.
- Virtual Environment: Python `venv` used for dependency isolation.
- CI/CD: Integrated GitHub Actions (`.github/workflows/unittests.yml`) to automate dependency validation and code linting.
- Commit History:Followed a descriptive commit strategy with frequent updates.

 2. Data Cleaning & Preprocessing
- Timestamp Standardization: Converted all news dates to UTC-standardized datetime objects.
- Publisher Normalization: Cleaned email-based publisher names to extract unique organizational domains.
- Deduplication: Removed redundant indices and entries to ensure statistical accuracy.

3. Key EDA Insights
- Publication Volume: Identified major news spikes (e.g., May 2013, Oct 2011) correlating with high market volatility.
- Temporal Patterns: Discovered a publication peak between 09:00 - 13:00 UTC, aligning with the U.S. Pre-Market session.
- Publisher Analysis: Identified that a small group of news organizations drives the majority of the dataset's volume.
- Text Analysis: Used TF-IDF to isolate top market themes like "Price Target" and "Earnings Beat," and LDA for topic clustering.
