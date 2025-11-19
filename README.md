Manchester United Midfield Dynamics
Bruno Fernandes & Casemiro Analysis (2025–26 Season Data)
Executive Summary

This project analyzes the on-pitch relationship between Bruno Fernandes and Casemiro during matches where both started for Manchester United in the 2025–26 Premier League season. Using match-level tables from FBref, we examine their per-90 profiles across creativity, progression, defensive impact, and involvement in possession.

The objective is to understand how their roles complement or diverge within Manchester United’s tactical structure, while demonstrating a modern, reproducible football-analytics workflow.

1. Why This Analysis Matters

Midfield structure strongly influences a team’s ability to control matches. Ball progression, defensive coverage, and possession value often hinge on how midfielders complement each other.

This analysis helps answer:

How much progression does Bruno provide relative to Casemiro?

Does Casemiro’s defensive output provide stability for Bruno’s creative freedom?

How consistent is their impact across different opponents?

What does their combined statistical profile reveal about United’s midfield balance?

2. Data Sources

All data originates from FBref match logs and player statistic tables.
Only matches where both players started in midfield are included.

Processed datasets:

midfield_matches_clean.csv

midfield_matches_features.csv

player_summary_per90.csv

Stored in the data/ directory.

3. Repository Structure

A clear, folder-based layout (no branch graphics):

Top-Level Folders

data/ – Raw and cleaned CSV stat tables

notebooks/ – All analysis notebooks, labeled in order

visuals/ – Exported PNG images used in the README and reports

README.md – Project documentation

Notebooks Overview

01_clean_data.ipynb – Merging and cleaning raw FBref tables

02_feature_engineering.ipynb – Per-90 calculations and feature creation

03_visualizations.ipynb – Progression and impact plots

04_radar_plots.ipynb – Radar charts for Bruno and Casemiro

05_extra_visuals.ipynb – Supplemental visuals (bar charts, role profiles)

Visual Exports

progression_split_elite.png

impact_map_elite.png

radar_bruno.png

radar_casemiro.png

radar_bruno_casemiro_overlay.png

match_dashboard_elite.png

role_profile_bruno_casemiro.png

4. Metrics Included
Progression and Creativity

Progressive passes per 90

Progressive carries per 90

Key passes per 90

Shot-creating actions per 90

Expected assists per 90 (when available)

Defensive Output

Tackles + interceptions per 90

Defensive actions

Pressure-related stats (future extension)

Possession and Involvement

Touches in key zones

Carry distances

Possession value (future extension)

All metrics are standardized to per-90 for fair comparison.

5. Visualizations
Progression Trends

Line plots showing match-by-match progression output for both players.

Creativity vs Defensive Impact Map

Scatter visualization mapping progression (x-axis) vs defensive output (y-axis).
Image: impact_map_elite.png

Radar Profiles

Individual and combined radars showing strengths across role-defining metrics.
Files: radar_bruno.png, radar_casemiro.png, radar_bruno_casemiro_overlay.png

Role Comparison Profiles

Scaled (0–1) bar charts comparing key progression and defensive categories.
Image: role_profile_bruno_casemiro.png

6. Additional Visuals (from 05_extra_visuals.ipynb)

Two supplemental visuals are included:

Average Per-90 Comparison Chart
Direct comparison of raw numerical output.

Role Comparison Bar Chart (Scaled)
Highlights relative strengths and differences between the two profiles.

These extend the analysis and provide a more club-style presentation layer.

7. Future Work

Expand analysis to full 2025–26 and 2026–27 seasons

Add full pressure metrics (PPDA, pressure regains, pressing zones)

Implement possession value models (VAEP, xThreat)

Construct dynamic passing networks and team shape diagrams

Add match-state segmentation and opponent contextualization

Build recruitment-style comparison radars vs league midfielders

8. License

This project is released under the MIT License.

Contact

Arnav Jain
Master of Science in Data Science, University of Virginia
LinkedIn: https://www.linkedin.com/in/arnavjain2026/

For collaboration, football-analytics roles, or feedback, feel free to connect.
