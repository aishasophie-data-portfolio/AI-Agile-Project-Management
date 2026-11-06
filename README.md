# AI-Agile-Project-Management
Master’s thesis on AI-augmented Agile Project Management: predicting sprint delays with Machine Learning and XGBoost, applying SHAP for explainability, and exploring AI routing mechanisms, human-in-the-loop decision-making, and AI governance.

## Overview

This project investigates how AI can support Agile teams in identifying delivery risks, understanding workflow patterns, and making  thoroughly tested project management decisions.
The research combines machine learning, operational data analysis, and real agile practitioner survey responses to develop an empirically grounded **AI-Augmented Agile Project Management Framework**.

The core idea is that AI tools should augment human expertise rather than replace human decision-making.
The human-in-the-loop approach served as the fundamental starting point for this research.

## Research Objectives

- **Predict:** Identify potential sprint delivery risks using machine learning.
- **Understand:** Analyse operational patterns in Agile workflows and user stories.
- **Contextualise:** Investigate agile practitioners' opinions of AI adoption, trust, and decision support.
- **Govern:** Development of a framework for successful AI implementation that integrates the aspects of explainability, human oversight, and AI governance into agile project management.

## Methodology

The study follows a mixed-methods approach, combining three complementary empirical perspectives.

### 1. Sprint Delay Risk Prediction

**Dataset:** JIRA Agile project data

- Data preprocessing and exploratory data analysis using Python.
- Feature engineering and classification model development.
- Comparison of a Multilayer Perceptron (MLP), Random Forest, and XGBoost.
- Model evaluation using metrics including macro F1-score and recall.
- Model interpretation using SHAP.
- Exploration of a Human-in-the-Loop routing approach for uncertain predictions.

**Key finding:** XGBoost achieved a macro F1-score of 0.895 and a recall of 0.925 for delayed sprint iterations on the independent test dataset. It demonstrated the potential of machine learning and in the case of the dataset, the tree model XGBoost, for identifying delivery risks in agile sprints.

### 2. Agile User Story Analysis

**Dataset:** User Story data

- Exploratory analysis of user story characteristics and story points.
- Investigation of patterns across Agile iterations.
- Examination of operational indicators that can contextualise AI-supported project decisions.

This analysis complements the predictive modelling by examining the operational context in which AI-generated insights may be used.

### 3. Practitioner Survey

**Dataset:** Survey responses from agile practitioners

The survey explores the human, organisational, and governance dimensions of AI adoption in Agile Project Management.

Key topics include:

- Trust in AI recommendations.
- Human oversight and accountability.
- Explainability and transparency.
- AI adoption and organisational readiness.
- Data privacy and governance.

Statistical methods include descriptive statistics, Cronbach's alpha, Wilcoxon signed-rank tests, Spearman rank correlations, effect sizes, and Holm correction where appropriate.

## 📂 Project Structure

AI-Agile-Project-Management/
├── README.md
└── notebooks/
    ├── README.md
    ├── 01_sprint_delay_prediction.ipynb
    └── 02_survey_analysis.ipynb


## 📊 Project Notebooks

 [Sprint Delay Prediction](notebooks/01_sprint_delay_prediction.ipynb) – Predictive modelling of sprint delays using machine learning.
 [Survey Analysis](notebooks/02_survey_analysis.ipynb) – Analysis of survey responses on AI adoption, trust, human-AI collaboration and AI governance.

## Technology Stack

- **Programming:** Python
- **Data Analysis:** Pandas, NumPy
- **Machine Learning:** MLP, Random Forest, XGBoost
- **Explainable AI:** SHAP
- **Visualisation:** Matplotlib
- **Analytics & Reporting:** Power BI
- **Research Methods:** Mixed-methods research, statistical hypothesis testing, exploratory data analysis

## Key Findings

- Machine learning can help identify potential sprint delivery risks.
- Model evaluation should reflect the business consequences of missed delays, not accuracy alone.
- Operational data provides context for interpreting predictive signals.
- Human oversight remains central to responsible AI-augmented decision-making.
- Explainability as a threshold for trust and organizational accountability are important factors for the acceptance 
and successful implementation of AI tools in agile organizations.

## Main Contribution: AI-Augmented Agile Project Management Framework

The principal contribution is an empirically derived framework that connects technical prediction with operational decision-making and responsible AI implementation.

The framework integrates:

1. **Business Challenge & Context** — defining the project management problem.
2. **AI-Augmented Decision Support** — generating predictive insights.
3. **Integration into Scrum Events** — embedding insights into Agile workflows.
4. **Governance, Explainability & Human Oversight** — ensuring accountable and human-in-the-loop approach.
5. **Business Value** — translating insights into more informed project decisions.

The framework positions AI as a decision-support capability within Agile teams, rather than as an autonomous replacement for project managers.

## Business Relevance

The research explores how organisations can use AI to:

- Identify delivery risks earlier.
- Support evidence-based sprint planning.
- Improve the interpretation of operational project data.
- Maintain human accountability for consequential decisions.
- Establish a responsible foundation for future AI and agentic AI applications.

## Limitations

The findings should be interpreted in the context of the available datasets, the exploratory nature of the research, and the limited survey sample. The framework is an empirically informed conceptual proposal; its effectiveness in live organisational environments requires further validation.

## Future Work

Potential next steps include:

- Validating the framework with real Agile teams.
- Testing the approach across different industries and project environments.
- Evaluating the impact of AI-supported decisions on delivery performance.
- Refining Human-in-the-Loop routing strategies.
- Investigating governance requirements for increasingly autonomous and agentic AI systems.

## Academic Context

This project was developed as part of a Master's degree in Business Analytics at Universidad Europea, Madrid.

**Research topic:** AI-Augmented Agile Project Management: A Framework for Enhancing Decision-Making, Performance, and Governance in
Business Analytics Environments.

## Author's Note

This project reflects my interest in Business Analytics, Machine Learning, Explainable AI, and responsible AI usage. My goal was, on the one hand, to demonstrate whether AI can generate useful predictions in agile PM. On the other hand, it was important to me to examine how these predictions can be integrated into a transparent and explainable decision-making tool for agile teams without replacing human oversight. The anonymous survey conducted by agile praktiker provided valuable insights into the conditions, under which AI can be used in agile organizations in a way that is long-term effective and increases efficiency. 
