Manchester United Midfield Dynamics: Bruno Fernandes & Casemiro Analysis (2024 Season Data)

This project analyzes Manchester United’s midfield performances when Bruno Fernandes and Casemiro both start together, using detailed match-level statistics extracted from FBref.
The purpose is to understand how their roles interact across possession, progression, creativity, and defensive actions, using a clean data pipeline and a professional analytics workflow suitable for a football club technical department.

1. Project Overview

This analysis focuses on all matches in which Bruno Fernandes and Casemiro started together. Data was scraped manually from FBref and organized into structured CSV files, then cleaned and merged into a unified analytical dataset.

Key objectives:

Build a reproducible data pipeline for match-level football analytics

Engineer per-90 statistics for fair comparison

Produce clear visualizations showing match-to-match dynamics

Generate professional radar charts comparing each player’s statistical profile

Highlight tactical insights relevant to their combined midfield contribution

The project is designed as a portfolio-ready case study for football data science roles.

2. Key Visuals

The following visuals are generated in the analysis notebooks and saved in the visuals/ directory.

Recommended visuals to showcase in the README (add exact filenames after exporting):

Progression Metrics Comparison (per 90)

Impact Comparison (xGChain, SCA, GCA, Defensive Actions)

Bruno Fernandes Radar

Casemiro Radar

Overlay Radar (Bruno vs Casemiro)

These visuals summarize the complementary profiles of both players and form the “story” of the analysis.

3. Tactical Insights

Based on the engineered metrics and visualizations:

Bruno Fernandes

Primary source of chance creation, final third progression, and shot-creating actions

High involvement in progressive passes and SCA/GCA chains

Operates as United’s most expansive playmaker across zones 2 and 3

Casemiro

Dominant in defensive actions per 90, especially tackles + interceptions

Carries the responsibility for central defensive stability and ball regains

Contributes to buildup through progressive carries and safe progression, not volume passing

Partnership Dynamics

Bruno advances possession and creates final-third value

Casemiro stabilizes transitions and defensive structure

Together, they create a balanced progression-and-protection model

Match patterns vary significantly by opponent and venue, which can be explored through the per-match trend plots

4. Data Pipeline

This project follows a clean, 4-notebook structure:

01_clean_data.ipynb

Loads all raw FBref exports

Standardizes column names

Cleans match metadata (dates, venues, competitions)

Merges Bruno + Casemiro stat tables

Produces: midfield_matches_clean.csv

02_feature_engineering.ipynb

Selects relevant features

Creates per-90 metrics for both players

Builds combined metrics for progression, creativity, and defensive actions

Produces:

midfield_matches_features.csv

player_summary_per90.csv

03_visualizations.ipynb

Match-to-match progression analysis

Creativity vs defensive involvement charts

Tactical visual summaries

Produces:

Line charts

Scatter/impact visuals

03_visualizations.pdf

04_radar_plots.ipynb

Radar profiles for Bruno and Casemiro

Standardizes selected per-90 stats on a 0–100 percentile scale

Produces:

radar_bruno.png

radar_casemiro.png

radar_overlay.png

04_radar_plots.pdf

5. Installation and Usage
Install dependencies

pip install -r requirements.txt

All notebooks are located in the notebooks/ directory.
Run them in numerical order:

01_clean_data.ipynb
02_feature_engineering.ipynb
03_visualizations.ipynb
04_radar_plots.ipynb

6. Folder Structure
project_root/
    data/
        raw_fbref_exports/
        midfield_matches_clean.csv
        midfield_matches_features.csv
        player_summary_per90.csv

    visuals/
        progression_plot.png
        impact_plot.png
        radar_bruno.png
        radar_casemiro.png
        radar_overlay.png

    notebooks/
        01_clean_data.ipynb
        02_feature_engineering.ipynb
        03_visualizations.ipynb
        04_radar_plots.ipynb

    reports/
        03_visualizations.pdf
        04_radar_plots.pdf

    README.md
    requirements.txt

   7. Future Work

Planned expansions include:

Adding full 2024–25 and 2025–26 season data

Incorporating pressure events (PPDA, pressure regains)

Creating a possession value model (xT or VAEP)

Adding positional heatmaps and zone-based influence charts

Using StatsBomb or Wyscout event data for deeper tactical layers

8. Purpose

This project is built as a professional-level football analytics case study with the aim of:

Demonstrating technical data science skills

Applying football domain knowledge

Producing visuals suitable for club reports

Building a strong foundation for a football analytics portfolio
