### NFL-PLayer-Stat-App

This app allows users to explore and compare NFL player stats across seasons through an interactive dashboard.

# Streamlit App

The Streamlit app is live at: https://nfl-player-stat-app.streamlit.app/

You can use the sidebar filters to select players and seasons, and generate stat comparisons. 

Key features:

Dropdowns to select players, positions, seasons
Interactive plots for seasonal comparisons
Tables summarizing key stats like passing yards, TDs
Ability to filter, sort and export data

# Model Training

The player data uses a Scraper script in data_scraper.py to pull latest stats from https://www.pro-football-reference.com

The data preprocessing pipeline cleans this data for model inputs. This includes:

- Handling missing values
- One-hot encoding positions
- Normalization of seasonal stats for comparison

  
# Deployment

The app is coded in Python using core Streamlit and Pandas libraries. 

Key highlights:

- Docker container for smooth deployment
- CI/CD GitHub Actions pipelines
- App monitoring via Streamlit cloud and Sentry

# Local Development

To run the app locally:

`pip install -r requirements.txt
streamlit run app.py`



# Dataset source: https://www.pro-football-reference.com

This app serves as a template for sports analytics use cases. The underlying data pipeline can be adapted for other statistical apps as well.
