# 🔥 MengAIo - Flamengo ML Analytics Project

**Comprehensive machine learning analytics for Flamengo across all competitions**

[![Python](https://img.shields.io/badge/python-v3.9+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Notion](https://img.shields.io/badge/integrated-Notion-black.svg)](https://notion.so)
[![FBref](https://img.shields.io/badge/data-FBref-orange.svg)](https://fbref.com)

> *Powered by AI, Driven by Passion* 🔴⚫

## 🏆 Competitions Covered

- **Brasileirão Série A**
- **Copa Libertadores**
- **Copa do Brasil**
- **Campeonato Carioca**
- **FIFA Club World Cup**

## 🚀 Quick Start

git clone https://github.com/your-username/MengAIo.git
cd MengAIo
pip install -r requirements.txt
cp .env.example .env   # add your keys
python scripts/pipelines/run_daily_update.py
streamlit run mengaio_dashboard.py

📁 Project Structure
mengaio/
├── scripts/        # Notion, scraping, features, ML models, pipelines
├── data/           # raw, processed, interim
├── models/         # trained models
├── outputs/        # charts, logs, reports
└── notebooks/      # Jupyter analysis notebooks

🛠️ Core Features
	•	Multi-competition analytics (Série A, Libertadores, etc.)
	•	Advanced ML models (XGBoost, baselines, classifiers)
	•	Notion integration (dashboards, player stats, match pages)
	•	Intelligent scraping (FBref Selenium automation with error handling)
	•	Production-ready pipeline (daily automation, modular design)

 🎯 Key Predictions
	•	Série A: final position, top 4 probability, points projection
	•	Libertadores: stage progression, champion probability, match outcome predictions
 
## 📊 Model Performance

| Competition  | Model Type         | Accuracy | Key Features                      |
|--------------|--------------------|----------|-----------------------------------|
| Série A      | Position Regressor | 84.3%    | Form, xG, Strength of Schedule    |
| Série A      | Top 4 Classifier   | 91.7%    | Points Projection, Goal Difference|
| Libertadores | Stage Classifier   | 78.9%    | Experience, Squad Value           |


🔧 Scripts Overview
# Scraping
python scripts/scraping/scrape_serie_a.py
python scripts/scraping/scrape_libertadores.py

# Feature Engineering
python scripts/features/build_match_features.py
python scripts/features/build_player_features.py

# ML
python scripts/models/train_baselines.py
python scripts/models/train_xgboost.py
python scripts/models/evaluate_models.py

# Notion
python scripts/notion/sync_match_pages.py
python scripts/notion/sync_player_pages.py
python scripts/notion/update_weekly_dashboards.py

# Pipelines
python scripts/pipelines/run_daily_update.py
python scripts/pipelines/backfill_seasons.py

📈 Data Sources
	•	FBref
	•	SofaScore
	•	Transfermarkt
	•	Notion API

 🔐 Environment
 NOTION_TOKEN=your_notion_token_here
SOFASCORE_API_KEY=your_sofascore_key
TRANSFERMARKT_API_KEY=your_transfermarkt_key

📊 Key Metrics Tracked

Match Level
	•	Goals For/Against, xG/xGA
	•	Possession, Shots, Pass Completion
	•	Defensive Actions, Progressive Passes
	•	Form indicators (last 5, 10 matches)

Player Level
	•	Goals, Assists, Minutes Played
	•	Shot Accuracy, Key Passes, Dribbles
	•	Defensive Actions, Aerial Duels
	•	Per-90 statistics

Advanced Analytics
	•	Goal difference trends
	•	Home/Away performance splits
	•	Strength of Schedule adjustments
	•	Head-to-Head records
 

🚀 Deployment
docker build -t mengaio .
docker run --env-file .env -p 8501:8501 mengaio

🤝 Contributing
	1.	Fork the repo
	2.	Create a feature branch (git checkout -b feature/amazing-feature)
	3.	Commit your changes (git commit -m 'Add amazing feature')
	4.	Push to the branch (git push origin feature/amazing-feature)
	5.	Open a Pull Request

⸻

📜 License

This project is licensed under the MIT License – see the LICENSE file for details.

⸻






