# Drowsiness Detection Datasets

This repository contains datasets prepared for research on **real-time driver drowsiness detection using facial landmarks and embedded AI**.

Repository URL:

`https://github.com/laurik-helshani/drowsiness`

## Dataset Files

### 1. `dataset_EAR_300.csv`
Contains 300 observations related to eye behavior.

Columns:
- `Timestamp_s` – timestamp in seconds
- `EAR` – Eye Aspect Ratio
- `Blinks_min` – estimated blink rate per minute
- `Label` – fatigue state/classification

### 2. `dataset_HeadPose_300.csv`
Contains 300 observations related to driver head pose.

Columns:
- `Timestamp_s` – timestamp in seconds
- `Yaw_deg` – horizontal head rotation in degrees
- `Pitch_deg` – vertical head rotation in degrees
- `Roll_deg` – head tilt in degrees
- `Label` – fatigue state/classification

### 3. `dataset_Physiology_300.csv`
Contains 300 observations related to fatigue indicators and driving behavior.

Columns:
- `Timestamp_min` – timestamp in minutes
- `PERCLOS_pct` – percentage of eye closure over time
- `SteeringError_deg` – steering deviation/error in degrees
- `Label` – fatigue state/classification

### 4. `Participant_Demographics_115.csv`
Contains demographic and experimental information for 115 synthetic participant profiles.

Columns:
- `Participant_ID` – unique participant identifier
- `Age` – participant age
- `Gender` – recorded gender
- `Eyewear` – whether eyewear was used
- `Skin_Tone` – synthetic skin-tone category
- `Driving_Experience_Years` – years of driving experience
- `Sleep_Hours_Before_Test` – sleep duration before testing
- `Environment` – experimental environment
- `Test_Type` – simulated or real-driving condition label

## Data Statement

The datasets are fully anonymized and contain no personally identifiable information. They are made available for research and educational purposes under an open license. 

## Intended Use

These datasets can be used for:
- Driver drowsiness detection research
- Eye Aspect Ratio (EAR) analysis
- PERCLOS-based fatigue analysis
- Head-pose analysis
- Fatigue classification
- Embedded AI and computer-vision experiments
- Statistical analysis and visualization

## Example: Loading a Dataset with Python

```python
import pandas as pd

df = pd.read_csv("dataset_EAR_300.csv")
print(df.head())
```

## Repository Structure

```text
drowsiness/
├── README.md
├── dataset_EAR_300.csv
├── dataset_HeadPose_300.csv
├── dataset_Physiology_300.csv
└── Participant_Demographics_115.csv
```

## Clone the Repository

After the files are pushed to GitHub, the repository can be downloaded with:

```bash
git clone https://github.com/laurik-helshani/drowsiness.git
cd drowsiness
```

## Citation

If you use these datasets in academic or research work, please cite the associated publication and reference this GitHub repository.

## Author

**Laurik Helshani**

GitHub: `https://github.com/laurik-helshani`
