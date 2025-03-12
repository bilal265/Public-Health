# Public-Health

NHANES is a program run by the CDC to assess the health and nutritional status of adults and children in the US. It combines survey questions and physical examinations, including medical and physiological measurements and laboratory tests, and examines a representative sample of about 5,000 people each year. The data is used to determine the prevalence of diseases and risk factors, establish national standards, and support epidemiology studies and health sciences research. This information helps to develop public health policy, design health programs and services, and expand the nation's health knowledge.

1. Dataset (https://raw.githubusercontent.com/HackBio-Internship/public_datasets/main/R/nhanes.csv)
2. Data Dictionary (https://github.com/HackBio-Internship/public_datasets/blob/main/R/nhanes_dd.csv)

## Key Findings
### Data Cleaning:
Null values were successfully handled using forward fill and default values, ensuring a complete dataset for analysis.

### Distributions (Histograms):
1. BMI: Likely shows a right-skewed distribution, typical for health data.
2. Weight (kg and lbs): Similar shape to BMI, with a possible peak around average adult weight.
3. Age: Could reveal the age range of the sample, possibly skewed toward older adults in NHANES data.
### Scatter Plots:
1. Weight vs. Height by Gender: Males (blue) might cluster at higher weights and heights than females (orange), reflecting biological differences.
2. Weight vs. Height by Diabetes: People with diabetes (red) may show higher weights or BMIs compared to those without (green).
3. Weight vs. Height by Smoking Status: Differences might be subtle, but current smokers (pink) could have lower weights than never smokers (purple).

### Statistical Insights:
1. Mean Pulse Rate: Provides a baseline (e.g., ~70-80 bpm if typical).
2. Diastolic BP Range: Indicates variability in blood pressure (e.g., a range of 50-60 mmHg might suggest diverse health statuses).
3. Income Variance/Std Dev: High values suggest significant income disparity in the sample.
### T-test Results:
1. Age vs. Gender: If p < 0.05, there’s a significant age difference between genders.
2. BMI vs. Diabetes: If p < 0.05, BMI differs significantly, likely higher in diabetic individuals.
3. Alcohol vs. Relationship Status: If p < 0.05, alcohol consumption varies by relationship status (e.g., singles might drink more).

### Summary
The code loads, cleans, and analyzes the NHANES dataset, producing visualizations and statistical tests to explore relationships between variables like weight, height, BMI, and demographic/health factors (gender, diabetes, smoking, etc.). Key findings depend on the actual data outputs (e.g., t-test p-values), but the code is designed to uncover patterns and differences in health metrics across subgroups.
