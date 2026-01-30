# Wine Quality Analysis (CART vs Random Forest)

## Overview
This project investigates **wine quality classification** using physicochemical measurements and compares an **interpretable Decision Tree (CART)** against a **Random Forest** model. To reflect real product/quality contexts, **red and white wines are modeled separately**, highlighting how feature distributions and decision boundaries differ across wine types.

## Objective
- Predict wine quality (ordinal classes) from chemical properties
- Compare **CART** (explainability) vs **Random Forest** (non-linear interactions)
- Address practical modeling issues such as **class imbalance** and **overlapping quality classes**
- Translate model outputs into **actionable quality-control insights**

## Dataset
- UCI **Vinho Verde** wine quality dataset (red & white variants)
- Inputs: physicochemical attributes (e.g., acidity, residual sugar, sulphates, alcohol, etc.)
- Target: wine quality score (multi-class / ordinal)

## Approach
### 1) Exploratory Data Analysis
- Distribution checks and summary statistics
- Feature relationships and redundancy/overlap between adjacent quality classes
- Red vs white comparison to motivate separate modeling

### 2) Modeling
**CART (Decision Tree)**
- Produces human-readable split rules
- Used to identify key drivers and threshold-style decision logic

**Random Forest**
- Captures non-linearities and feature interactions
- Used for stronger predictive stability and generalization

### 3) Evaluation
- Classification performance metrics (e.g., accuracy / balanced accuracy / kappa where applicable)
- Confusion matrix review to understand where models confuse adjacent quality levels
- ROC-based review (where applicable) and threshold considerations
- Class imbalance handling (e.g., class weighting) to reduce majority-class bias

## Key Findings (Summary)
- **Random Forest** generally performs better than CART in overall stability and predictive power due to non-linear interactions.
- **CART** remains valuable for **interpretability**, offering clear decision rules and feature thresholds.
- **Class imbalance** and **feature overlap** make minority/adjacent quality classes harder to separate; weighting and careful metric selection are important.
- Red and white wines show **different feature–quality relationships**, supporting the decision to model them separately.

## Deliverables
- `Wine Quality Analysis.pdf` — full report (methods, results, discussion)

## How to view the report
- Open `Wine Quality Analysis.pdf` directly in GitHub (if preview is available), or click **Download** to view locally.
- Tip: if GitHub preview fails, rename the file to remove spaces (e.g., `wine-quality-analysis.pdf`) and re-upload.

## Repository Contents
- `README.md` — project summary
- `Wine Quality Analysis.pdf` — report (primary deliverable)

## Author
Shu-Yu Lin
