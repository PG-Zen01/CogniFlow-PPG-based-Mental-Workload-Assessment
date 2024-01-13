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

### Step 4: Training and Classification

- Assigned 30% of the dataset for testing purposes.

- Employed Support Vector Machine (SVM) for classification.

- Tuned the regularization parameter (C) to 600 for optimal performance.
