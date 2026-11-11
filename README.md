# AI-Augmented Agile Project Management

**Master’s thesis | Business Analytics | Machine Learning | Explainable AI | AI Governance**

How can AI support Agile teams in identifying sprint delivery risks, improving decision-making, and integrating predictive insights into project management while keeping humans in control?

This project combines machine learning, operational data analysis, and survey research to develop an **AI-Augmented Agile Project Management Framework** for responsible, data-driven decision support.

The central principle: AI should augment human expertise, not replace human judgment.

## Overview

The project explores two complementary perspectives:

- **Technical perspective:** Predicting sprint delays using machine learning, evaluating model performance, and investigating explainability and human-in-the-loop routing.
- **Human and organisational perspective:** Analysing Agile practitioners’ responses concerning AI adoption, trust, transparency, human oversight, and governance.

Together, these perspectives inform a conceptual framework for integrating AI into Agile project management.

## Research Questions

- Can sprint delivery risks be predicted from information intended to be available at sprint start?
- How do Random Forest, XGBoost, and a Multilayer Perceptron (MLP) compare on the available dataset?
- How can model explanations and confidence-based routing support human review?
- What do Agile practitioners report about AI efficiency, trust, explainability, and governance?

## Research Objectives

- **Predict:** Identify potential sprint delivery risks using machine learning.
- **Understand:** Examine predictive performance and the factors associated with model predictions.
- **Contextualise:** Investigate practitioners’ perspectives on AI adoption, trust, and decision support.
- **Govern:** Develop a framework integrating explainability, human oversight, and responsible AI governance.

## Methodology

The research follows a mixed-methods approach, combining predictive modelling with survey-based statistical analysis.

### 1. Sprint Delay Risk Prediction

**Dataset:** JIRA Agile project data

The technical analysis includes:

- Data preprocessing and exploratory data analysis (EDA).
- Feature engineering and classification.
- Comparison of Random Forest, XGBoost, and a Multilayer Perceptron (MLP).
- Model evaluation using macro F1-score, recall, and other classification metrics.
- Model explainability using SHAP.
- Exploration of a human-in-the-loop routing approach for uncertain predictions.

**Key result**

XGBoost achieved a macro F1-score of **0.895** and a recall of **0.925** for delayed sprint iterations on the independent test dataset.

These results demonstrate promising predictive performance on the available data. Further validation would be required before applying the model in a live project management environment.

### 2. Agile Practitioner Survey Analysis

**Dataset:** Survey responses from Agile practitioners

The survey investigates human, organisational, and governance-related dimensions of AI adoption in Agile project management.

Key topics include:

- Trust in AI recommendations.
- Human oversight and accountability.
- Explainability and transparency.
- AI adoption and organisational readiness.
- Data privacy and governance.

Statistical methods include:

- Descriptive statistics.
- Cronbach’s alpha for internal consistency.
- Wilcoxon signed-rank tests.
- Spearman rank correlations.
- Effect sizes and Holm correction, where appropriate.

The survey analysis complements the technical modelling by examining the perspectives and concerns that may influence the adoption of AI-supported decision-making.

**Research limitation:** The survey has a limited sample size. Its findings should therefore be interpreted as exploratory rather than representative of all Agile practitioners.

## Project Structure

AI-Agile-Project-Management/
├── README.md
└── notebooks/
    ├── README.md
    ├── 01_sprint_delay_prediction_portfolio.ipynb
    └── 02_survey_analysis_portfolio.ipynb


## Project Notebooks

**01 — [Sprint Delay Prediction](notebooks/01_sprint_delay_prediction_portfolio.ipynb)**

Predictive modelling, model comparison, evaluation, and explainability for sprint delivery risk.

**02 — [Survey Analysis](notebooks/02_survey_analysis_portfolio.ipynb)**

Statistical analysis of Agile practitioners’ perspectives on AI adoption, trust, human-AI collaboration, and governance.


## Technology Stack

- **Programming:** Python
- **Data Analysis:** Pandas, NumPy
- **Machine Learning:** Scikit-learn, Random Forest, XGBoost, MLP
- **Explainable AI:** SHAP
- **Visualisation:** Matplotlib
- **Statistical Analysis:** SciPy, hypothesis testing, effect sizes
- **Research Methods:** Exploratory data analysis, mixed-methods research

## Key Findings and Implications

- Machine learning can help identify potential sprint delivery risks in the available dataset.
- Model evaluation should consider the consequences of missed delays, not accuracy alone.
- Explainability can help practitioners understand model predictions and assess their relevance.
- Human oversight remains important when AI-generated insights inform consequential decisions.
- Organisational readiness, trust, transparency, and governance are relevant considerations for AI adoption.

These findings inform a proposed framework rather than demonstrating that AI adoption will automatically improve delivery performance.

## Main Contribution: AI-Augmented Agile Project Management Framework

The principal contribution is a conceptual framework connecting predictive insights with operational decision-making and responsible AI implementation.

The framework consists of five components:

1. **Business Challenge & Context** — Define the project management problem and relevant business objectives.
2. **AI-Augmented Decision Support** — Generate predictive insights to inform project decisions.
3. **Integration into Scrum Events** — Consider how AI insights could support sprint planning, reviews, and retrospectives.
4. **Governance, Explainability & Human Oversight** — Support transparency, accountability, and human review.
5. **Business Value** — Evaluate whether AI-supported decisions contribute to better-informed project management.

The framework positions AI as a decision-support capability within Agile teams, not as an autonomous replacement for project managers.

## Business Relevance

The research explores how organisations could use AI to:

- Identify delivery risks earlier.
- Support evidence-informed sprint planning.
- Interpret operational project data more effectively.
- Maintain human accountability for important decisions.
- Establish a foundation for responsible future AI applications.

## Limitations

The results are subject to the limitations of the available datasets, the modelling approach, and the exploratory survey design.

Predictive performance on a test dataset does not guarantee generalisation to other organisations or projects. Survey findings from a limited sample cannot be assumed to represent the wider Agile community. The proposed framework requires further evaluation with real Agile teams before its practical effectiveness can be established.

## Future Work

Potential next steps include:

- Validating the predictive approach across different project environments.
- Evaluating the framework with Agile practitioners and project teams.
- Refining confidence-based human-in-the-loop routing strategies.
- Investigating the impact of AI-supported decisions on delivery performance.
- Exploring governance requirements for increasingly autonomous AI systems.

## Academic Context

Developed as part of the Master’s degree in Business Analytics at Universidad Europea, Madrid.

**Thesis title:** *AI-Augmented Agile Project Management: A Framework for Enhancing Decision-Making, Performance, and Governance in Business Analytics Environments.*

## About This Project

This project reflects my interest in Business Analytics, Machine Learning, Explainable AI, and responsible AI adoption.

My goal was to investigate both the predictive potential of AI in Agile project management and the conditions under which its recommendations can be integrated into transparent, human-centred decision-making.

By combining technical analysis with practitioner perspectives, I explored how AI can support more informed decisions while preserving human judgment and accountability.

**Technologies:** Python · Machine Learning · XGBoost · SHAP · Statistical Analysis · AI Governance
