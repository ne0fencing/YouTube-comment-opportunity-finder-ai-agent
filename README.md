# YouTube Comment Opportunity Finder AI Agent

https://run.relay.app/shared/youtube-comment-opportunity-finder-7jUPhyX9r0hg

## 🚀 Project Overview
This project is an AI-powered agent designed to help YouTube creators engage with their community effectively. It automatically filters out spam, cleans messy data, identifies genuine questions, and drafts high-quality replies for human approval.

## 🛠️ Technology Stack
- **AI Model:** Google Flan-T5 (via Hugging Face)
- **Data Engineering:** IBM Data Prep Kit (DPK)
- **Automation:** Relay.app
- **Language:** Python 3.10+

## 📂 Repository Structure
- `data/`: Contains `raw_comments.csv` and `comments_clean.parquet`.
- `src/agent.py`: The reasoning logic (Phase 1).
- `src/data_processor.py`: The DPK cleaning script (Phase 2).
- `src/app_integration.py`: The handover logic for Relay.app (Phase 3).

## 📈 The 3-Phase Pipeline
1. **Phase 1 (Logic):** A reasoning loop that evaluates comments to decide if they are "Engagement Opportunities."
2. **Phase 2 (Data Prep):** Implementation of deduplication and noise removal using IBM Data Prep Kit principles to ensure data quality.
3. **Phase 3 (Automation):** A live workflow using Relay.app that sends a Gmail notification whenever a high-value question is found.
