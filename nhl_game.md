
# 🏒 NHL Game Analytics Data Platform
# 📌 Project Overview

Built an end-to-end ELT data platform transforming 20 years of NHL historical game data (12 CSV datasets) into an analytics-ready dimensional model powering executive dashboards.

Objective:
Design a scalable data pipeline and deliver performance intelligence for coaches, analysts, and operations teams.

# 🏗 Architecture Design

Implemented a Medallion Architecture:

# 🥉 Bronze Layer

Raw data ingestion (CSV → Delta Tables)

Minimal transformation

Referential integrity validation

Preserved source fidelity

# 🥈 Silver Layer

Data cleansing & standardization

Deduplication

Attribute normalization

Granularity alignment

Analytical enrichment

This structure ensured modular transformation, traceability, and scalable reprocessing.

# 🧱 Dimensional Data Model

Designed an analytics-ready semantic model:

Fact Tables:

Game Events

Player Statistics

Goalie Statistics

Shift Data

Dimension Tables:

Teams

Players

Game

Date

Optimized relationships for:

Performance analytics

Time-on-ice normalization

Cross-game comparisons

Team vs player benchmarking

# 📊 Metrics Engineering

Key analytical enhancements:

Performance normalized per 60 minutes of time-on-ice

League average benchmarking

Regulation vs OT/SO point logic modelling

Season-level trend normalization

Designed metrics to avoid bias from uneven playtime distribution.

# 📈 Power BI Strategy

Design Principles:

Minimal clutter

Consistent slicers

Role-based insight delivery

Dashboards Built:

League Overview

Team Performance

Skater Efficiency

Goalie Performance

League Trend Analysis

Focused on decision intelligence — not just visualization.

# 🤖 Machine Learning POC

Built binary classification model predicting match outcomes

Identified skewed probability distributions

Resolved scaling issue affecting early prediction confidence

Demonstrated feature impact on win probability

# ⚠ Challenges & Improvements

Challenges:

Incomplete source identifiers

Schema rigidity after semantic model lock-in

Compute limitations in trial environment

Future Enhancements:

Pipeline logging & monitoring

Shift-level workload analysis

Shot coordinate spatial analytics

Home vs Away performance modelling

# 🎯 Key Engineering Takeaways

Data modelling decisions directly affect downstream flexibility

Early schema design must anticipate analytical expansion

Visualization logic should be integrated back into transformation layers

Performance normalization is critical for fair comparison
