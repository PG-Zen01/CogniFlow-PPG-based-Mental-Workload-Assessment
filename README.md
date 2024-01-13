# CogniFlow-PPG-based-Mental-Workload-Assessment

## Overview

Stress is a significant concern in modern societies, impacting productivity, health, and cardiovascular well-being. This project introduces a novel approach to estimate stress levels using Photoplethysmogram (PPG) signals.

## Why PPG?

- **Non-Invasive Method:** PPG signals provide a comfortable and non-intrusive way to monitor physiological data.
  
- **Low Cost:** PPG sensors are cost-effective, making stress monitoring accessible to a broader audience.

- **Easy to Measure:** PPG signals can be easily obtained using common devices with integrated sensors or dedicated wearables.

## Objectives

1. **IMF Extraction from PPG Signal:**
   - Decompose PPG signals into Intrinsic Mode Functions (IMFs) to capture underlying stress-related patterns.

2. **Feature Extraction from IMF:**
   - Identify relevant features within the extracted IMFs that correlate with stress levels.

3. **Stress Estimation:**
   - Utilize the extracted features for stress estimation, providing a quantitative measure of stress levels.

## Methodology

### Step 1: Data Collection

- Utilized the publicly available MAUS dataset for research purposes.

### Step 2: Data Preprocessing

- Segregated data into low and high-stress categories.
  
- Merged data from all 22 individuals to create a comprehensive dataset.

- Applied StandardScaler to normalize the data.

### Step 3: Empirical Mode Decomposition (EMD) for Feature Extraction

- Decomposed PPG signals into IMFs using Empirical Mode Decomposition, revealing stress-related patterns.

  ![image](https://github.com/PG-Zen01/CogniFlow-PPG-based-Mental-Workload-Assessment/assets/156335467/66d21da4-8f25-4106-9068-6f43081e3e02)

![image](https://github.com/PG-Zen01/CogniFlow-PPG-based-Mental-Workload-Assessment/assets/156335467/21309edb-5d4f-4f52-a8b3-2e1cc5a0bca6)



### Step 4: Training and Classification

- Assigned 30% of the dataset for testing purposes.

- Employed Support Vector Machine (SVM) for classification.

- Tuned the regularization parameter (C) to 600 for optimal performance.

##Correlation matrix
![image](https://github.com/PG-Zen01/CogniFlow-PPG-based-Mental-Workload-Assessment/assets/156335467/ba319dd6-78e1-479e-be63-0fcc6466167a)

##Confusion matrix
![image](https://github.com/PG-Zen01/CogniFlow-PPG-based-Mental-Workload-Assessment/assets/156335467/fd740d4f-895c-4eb4-be66-8c6d9cc31d69)


