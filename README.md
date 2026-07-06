# AI-Assisted Workspace Planning Intelligence System

## Overview

A BIM-integrated decision support system that evaluates office workspace layouts using architectural planning heuristics and machine learning.

This project combines **Architecture + BIM + Data Science** by transforming subjective workspace planning decisions into measurable spatial performance indicators.

---

## Objectives

- Extract workspace metrics from a Revit model
- Evaluate layouts using architectural planning rules
- Calculate a weighted spatial efficiency score
- Predict layout efficiency using Machine Learning
- Generate automated design recommendations

---
## Methodology

### 1. BIM Data Extraction

The office workspace was modeled in **Autodesk Revit**, and key spatial metrics were extracted using room and furniture schedules.

**Extracted Metrics**
- Room Areas
- Occupancy
- Area per Person
- Circulation Percentage
- Functional Space Categories
- Workspace Adjacency

---

### 2. Rule-Based Workspace Evaluation

Seven architectural planning heuristics were developed to evaluate each layout.

| Rule | Weight |
|------|-------:|
| Meeting Adjacency | 20 |
| CEO ↔ Conference Accessibility | 15 |
| Cabin Proximity | 15 |
| Circulation Efficiency | 20 |
| Crossing Flow | 10 |
| Density | 10 |
| Pantry Zoning | 10 |

Each layout is scored using these weighted rules to generate an overall workspace efficiency rating.

---

### 3. Spatial Efficiency Scoring

The weighted rule scores are combined into a single **Efficiency Score (0–100)**, allowing objective comparison between multiple workspace layouts.

| Layout | Efficiency Score |
|--------|-----------------:|
| Layout A | 61.5 |
| Layout B | 73.0 |
| Layout C | 69.5 |

---

### 4. Machine Learning

A **Linear Regression** model was trained using the architectural evaluation scores to predict workspace efficiency for different layout configurations.

---

### 5. Automated Design Recommendations

Based on the evaluated layouts, the system generates recommendations such as:

- Improve meeting room accessibility
- Reduce excessive circulation area
- Relocate pantry away from focused workspaces
- Increase area per person to improve comfort
- Improve spatial relationships between key functional spaces


---

## Workflow

```text
Revit Model
      ↓
Room & Furniture Schedules
      ↓
Spatial Metrics Extraction
      ↓
Rule-Based Evaluation
      ↓
Efficiency Score
      ↓
Machine Learning
      ↓
Design Recommendations
```

---

## Features

- BIM data extraction from Revit
- Rule-based workspace evaluation
- Weighted efficiency scoring
- Linear Regression model
- Automated design recommendations
- Data visualization using Matplotlib

---

## Tools & Technologies

- Autodesk Revit
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## Results

- Compared multiple office layout alternatives
- Quantified workspace efficiency using architectural heuristics
- Predicted layout performance using Machine Learning
- Generated explainable recommendations for design improvement

---

## Repository Structure

```
├── data/
├── notebooks/
├── images/
├── README.md
└── requirements.txt
```

---

## Skills Demonstrated

**Architecture:** Space Planning • Workplace Design • Spatial Analysis

**BIM:** Revit • Schedule Extraction • Data Structuring

**Data Science:** Python • Machine Learning • Data Visualization

---

*This project demonstrates the application of BIM, architectural decision-making, and data science to support evidence-based workspace planning.*
