# Personal Chat Moderation System

## Project Overview
This is a comprehensive chat moderation system designed to analyze and filter inappropriate content using machine learning techniques.

## System Requirements

Python 3.8+

## Required Python Packages:

+ flask
+ transformers
+ torch
+ pandas
+ scikit-learn
+ sqlite3
+ flask-cors

## Project Structure
## Core Application Files

+ run.py: Main entry point to start the Flask application (not in use for now)
+ config.py: Configuration management for the application
+ app/__init__.py: Flask application initialization

## Moderation Components

+ app/main.py: Core application logic and server configuration
+ app/routes.py: API endpoints for content moderation
+ app/models.py: Database models and machine learning model definitions
+ app/database.py: Database connection and interaction methods
+ app/utils.py: Utility functions for text processing and analysis

## Machine Learning

+ app/train_jigsaw_model.py: Model training script for text classification
+ app/testing.py: Model testing and evaluation script
+ app/templates/jigsaw_results/: Contains model checkpoints and visualization results

## Frontend

+ app/templates/frontend.html: Web interface for the moderation system
+ app/style.css: Styling for the web interface

## Model Capabilities

The system uses a fine-tuned BERT model to detect:

+ Toxic comments
+ Severe toxic content
+ Obscene language
+ Threats
+ Insults
+ Identity-based hate speech

## Performance Metrics

Detailed performance metrics are available in the PERFORMANCE METRICS/ directory, showing:

+ Classification accuracy
+ Confusion matrices
+ ROC curves
+ Latency analysis

## Database

+ moderation_logs.db: SQLite database for storing moderation logs and user interactions
