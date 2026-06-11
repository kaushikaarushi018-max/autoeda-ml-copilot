# 🧠 AutoEDA — ML Copilot

An end-to-end, browser-based data science tool that turns any CSV into instant insights — no backend, no installation, no cost.

🔗 **Live demo:** https://kaushikaarushi018-max.github.io/autoeda-ml-copilot/

## Features

- 📋 **Automated Data Profiling** — instantly detects column types, missing values, cardinality, and data quality issues
- 📊 **Auto-Generated Visualizations** — histograms, categorical bar charts, and a correlation heatmap, dynamically built for any dataset
- 🤖 **AI Data Narrative** — Claude (Anthropic) reads the dataset's statistics and writes a human-readable analyst report
- 🌲 **In-Browser Machine Learning** — trains a Random Forest (classifier or regressor, auto-detected) entirely in JavaScript, with accuracy/precision/recall/R²/feature importance — no server required
- 💬 **Conversational Data Q&A** — chat with your dataset in plain English; Claude has full context on stats, correlations, and model results

## Tech Stack

- Vanilla JavaScript, HTML, CSS (no frameworks, no build step)
- PapaParse for CSV parsing
- Chart.js for visualizations
- Custom-built Random Forest implementation (decision trees, bootstrap aggregation, Gini-based feature importance)
- Anthropic Claude API for narrative generation and chat

## How it works

1. Upload any CSV
2. The app auto-detects numeric vs. categorical columns and profiles the dataset
3. Visualizations and a correlation heatmap are generated automatically
4. Pick a target column — the app trains a Random Forest and shows performance metrics
5. Ask questions about your data in the chat — Claude has full context

## Privacy

This app runs **entirely in your browser**. Your data never leaves your machine except when you choose to use the AI features (Steps 3 & 5), which call the Anthropic API directly using your own API key. No backend, no data storage, no tracking.

## Why I built this

As a data scientist, I wanted to demonstrate the full pipeline — from raw data to deployed model to AI-powered insights — in a single, accessible tool that anyone can use without setup.
