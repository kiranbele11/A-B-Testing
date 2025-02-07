# A/B Testing Analysis Project

## Overview
This project demonstrates a comprehensive A/B testing analysis for an e-commerce website's product page redesign. The analysis evaluates whether a new design leads to improved conversion rates compared to the existing design.

## Business Case
- **Current Scenario**: E-commerce platform with 13% baseline conversion rate
- **Goal**: Evaluate if a new UX design can increase conversion rate by 2% (to 15%)
- **Test Type**: Two-sample proportion test (A/B test)

## Technical Implementation
### Technologies Used
- Python 3.12
- Key Libraries:
  - NumPy: Numerical computations
  - Pandas: Data manipulation
  - SciPy: Statistical testing
  - Statsmodels: Statistical analysis
  - Matplotlib & Seaborn: Data visualization

### Statistical Methods
- Power Analysis for sample size determination
- Z-test for proportion comparison
- Confidence Interval calculation
- Statistical significance testing (α = 0.05)

## Key Findings
1. **Sample Size**: Required 4,720 observations per group for statistical validity
2. **Conversion Rates**:
   - Control Group: 12.3%
   - Treatment Group: 12.6%
3. **Statistical Results**:
   - p-value: 0.732 (> α = 0.05)
   - 95% Confidence Intervals:
     - Control: [11.4%, 13.3%]
     - Treatment: [11.6%, 13.5%]

## Methodology
1. **Experiment Design**
   - Defined control (old design) and treatment (new design) groups
   - Implemented binary success metric (converted: 0/1)
   - Calculated required sample size using power analysis

2. **Data Collection & Cleaning**
   - Cleaned and preprocessed raw data
   - Removed duplicate user sessions
   - Ensured balanced sample sizes between groups

3. **Statistical Analysis**
   - Conducted hypothesis testing
   - Calculated confidence intervals
   - Performed visualization of results

## Conclusions
- No statistically significant difference between the two designs
- Failed to achieve the target 2% improvement
- New design does not justify implementation based on conversion metrics

## Learning Outcomes
1. **Statistical Analysis**:
   - Practical application of hypothesis testing
   - Understanding of power analysis
   - Confidence interval interpretation

2. **Data Science Skills**:
   - Data manipulation with Pandas
   - Statistical visualization
   - Python programming for analysis

3. **Business Insights**:
   - A/B testing methodology
   - Data-driven decision making
   - Statistical significance in business context

## Setup and Installation
1. Create a virtual environment:
   ```bash
   python -m venv abnenv
   ```
2. Activate the environment:
   ```bash
   source abnenv/bin/activate  # Unix/macOS
   .\abnenv\Scripts\activate   # Windows
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Future Improvements
- Include additional metrics beyond conversion rate
- Implement segmentation analysis
- Add visualization of confidence intervals
- Consider multivariate testing approaches


