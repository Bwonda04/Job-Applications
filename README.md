# Concept Drift Detection in ML Systems

A research implementation of statistical drift detection methods for monitoring 
machine learning model reliability in non-stationary environments.

## Overview

This project investigates how machine learning models degrade over time when 
the underlying data distribution shifts — a phenomenon known as concept drift. 
Using real-world datasets, we implement and evaluate drift detection algorithms 
from first principles to characterize model robustness under distribution shift.

Built as part of CSCI 4144 Data Mining and Data Warehousing at Dalhousie University.

## Methods

- **DDM (Drift Detection Method)** — implemented from first principles based on 
  Žliobaitė (2010), using incremental error rate tracking with warning and drift 
  thresholds at 2σ and 3σ
- **Sliding Window Evaluation Framework** — custom pipeline for evaluating 
  classifier performance across time windows on non-stationary data streams

## Datasets

- **ELEC2** — electricity demand dataset with real-world concept drift
- **SEA Concepts** — synthetic benchmark for evaluating drift detection under 
  controlled distribution shift

## Key Findings

- Evaluated trade-offs between detection latency and false alarm rate under 
  varying drift speeds and magnitudes
- Characterized model robustness metrics including accuracy degradation and 
  recovery time post-drift

## Tech Stack

Python, Scikit-learn, Pandas, NumPy, R

## Authors

Basit Abaniwonda — ddm.py, evaluator.py, data pipeline
