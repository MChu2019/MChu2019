
# 🏒 NHL Game Analytics Data Platform
# 📌 Project Overview

Built an end-to-end ELT data platform transforming 20 years of NHL historical game data (12 CSV datasets) into an analytics-ready dimensional model powering executive dashboards.

Objective:
Design a scalable data pipeline and deliver performance intelligence for coaches, analysts, and operations teams.

# 🏗 Architecture Design

Implemented a Medallion Architecture:

# 🥉 Bronze Layer

Raw data ingestion (CSV → Delta Tables)<br>
Minimal transformation<br>
Referential integrity validation<br>
Preserved source fidelity

# 🥈 Silver Layer

Data cleansing & standardization<br>
Deduplication<br>
Attribute normalization<br>
Granularity alignment<br>
Analytical enrichment

This structure ensured modular transformation, traceability, and scalable reprocessing.

# 🧱 Dimensional Data Model

Designed an analytics-ready semantic model:<br>

Fact Tables:<br>
Game Events<br>
Player Statistics<br>
Goalie Statistics<br>
Shift Data

Dimension Tables:<br>
Teams<br>
Players<br>
Game<br>
Date

Optimized relationships for:<br>
Performance analytics<br>
Time-on-ice normalization<br>
Cross-game comparisons<br>
Team vs player benchmarking

# 📊 Metrics Engineering
Key analytical enhancements:<br>
Performance normalized per 60 minutes of time-on-ice<br>
League average benchmarking<br>
Regulation vs OT/SO point logic modelling<br>
Season-level trend normalization

Designed metrics to avoid bias from uneven playtime distribution.

# 📈 Power BI Strategy

Design Principles:<br>
Minimal clutter<br>
Consistent slicers<br>
Role-based insight delivery

Dashboards Built:<br>
League Overview<br>
Team Performance<br>
Skater Efficiency<br>
Goalie Performance<br>
League Trend Analysis

Focused on decision intelligence — not just visualization.

# 🤖 Machine Learning POC

Built binary classification model predicting match outcomes<br>
Identified skewed probability distributions<br>
Resolved scaling issue affecting early prediction confidence<br>
Demonstrated feature impact on win probability

# ⚠ Challenges & Improvements

Challenges:

Incomplete source identifiers<br>
Schema rigidity after semantic model lock-in<br>
Compute limitations in trial environment

Future Enhancements:

Pipeline logging & monitoring<br>
Shift-level workload analysis<br>
Shot coordinate spatial analytics<br>
Home vs Away performance modelling

# 🎯 Key Engineering Takeaways

Data modelling decisions directly affect downstream flexibility<br>
Early schema design must anticipate analytical expansion<br>
Visualization logic should be integrated back into transformation layers<br>
Performance normalization is critical for fair comparison
