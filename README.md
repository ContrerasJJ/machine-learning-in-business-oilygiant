# Machine Learning in Business: Oil Well Profit Optimization (OilyGiant)

## Table of Contents
- [Project Objective](#project-objective)
- [Project Structure](#project-structure)
- [Tools and Techniques Utilized](#tools-and-techniques-utilized)
- [Results and Recommendations](#results-and-recommendations)
- [What I Have Learned From This Project](#what-i-have-learned-from-this-project)
- [How to Use This Repository](#how-to-use-this-repository)

---

## Project Objective

You work for the mining company **OilyGiant**. The goal of this project is to use machine learning and statistical analysis to determine the most profitable region for drilling a new oil well. 

Using data from three potential regions, the project:

- Predicts the volume of reserves in each well,
- Calculates expected profit,
- Estimates the **risk of financial loss** for each region.

---

## Project Structure

1. **Data Loading and Preparation**
   - Loaded datasets for three oil regions.
   - Checked for missing values, anomalies, and basic statistics.
   - Split data into train and validation sets for each region.

2. **Model Training and Evaluation**
   - Trained a **Linear Regression** model to predict oil reserves in each region.
   - Evaluated model quality using **RMSE** and average predicted reserves.
   - Compared performance across regions.

3. **Profit Calculation**
   - Used business constraints (number of wells to select, budget, revenue per thousand barrels) to calculate expected profit.
   - Selected the top wells in each region based on predicted reserves.
   - Computed expected profit distributions.

4. **Risk Assessment with Bootstrapping**
   - Applied **bootstrapping** (1,000 iterations) to model the distribution of profits.
   - Estimated:
     - Average profit per region.
     - 95% confidence intervals.
     - Probability of loss for each region.

5. **Final Region Selection**
   - Selected the region with the highest expected profit and acceptable risk profile.

---

## Tools and Techniques Utilized

- **Programming & Libraries**
  - Python, Jupyter Notebook
  - pandas, NumPy
  - scikit-learn (Linear Regression)
  - matplotlib, seaborn

- **Methods**
  - Regression modeling
  - Train/validation split
  - Error metrics (RMSE)
  - Profit and loss calculations
  - Bootstrapping for risk estimation
  - Confidence intervals

---

## Results and Recommendations

- Built a regression model to predict oil reserves with reasonable accuracy for each region.
- Calculated the expected profit for each region based on model predictions and business constraints.
- Estimated the probability of financial loss using bootstrapping.

**Key Results (example structure – fill in with your actual numbers):**
- Region A: Average profit = `X` ; Probability of loss = `Y%`
- Region B: Average profit = `X` ; Probability of loss = `Y%`
- Region C: Average profit = `X` ; Probability of loss = `Y%`

**Final Recommendation:**

Select **the region with the highest expected profit and a loss probability below the acceptable threshold (e.g., 2.5%)** for drilling the new oil well.

---

## What I Have Learned From This Project

- How to connect machine learning models directly to **business metrics** like profit and risk.
- The importance of combining predictions with **financial constraints** rather than only focusing on error metrics.
- How **bootstrapping** can be used to estimate risk and uncertainty in profit calculations.
- Practical experience in using regression for real-world decision-making.

---

## How to Use This Repository

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ContrerasJJ/machine-learning-in-business-oilygiant.git
   cd machine-learning-in-business-oilygiant
