---
layout: project
type: project
image: https://o.aolcdn.com/images/dims?thumbnail=960%2C&quality=95&image_uri=https%3A%2F%2Fs.yimg.com%2Fuu%2Fapi%2Fres%2F1.2%2FqEjW8LMkT.vPxSm7ekRC8A--%7EB%2FaD0xMzM0O3c9MjAwMDthcHBpZD15dGFjaHlvbg--%2Fhttps%3A%2F%2Fo.aolcdn.com%2Fimages%2Fdims%3Fresize%3D2000%252C2000%252Cshrink%26image_uri%3Dhttps%253A%252F%252Fs.yimg.com%252Fos%252Fcreatr-uploaded-images%252F2019-06%252F29d9e1e0-8d17-11e9-badf-8e6de9f73ea9%26client%3Da1acac3e1b3290917d92%26signature%3D370ce1f3213dc3ed909feabe79c9ef9f16a7a129&client=amp-blogside-v2&signature=08a850af9af537cf5ffccbe7138f0c71628b7229
title: Regression Model to Predict Patient Estimated Hospitalization Time
permalink: projects/Drug-Regression-Model
date: 2020
labels:
  - Python
  - Clinical Data
  - Regression Model
Summary: Built a machine learning model to identify diabetes patients that are likely to be treated with a client drug, thereby ensuring effective reach out of the medical representatives to the corresponding physicians.
---

### Project Overview
Drugs that are ready for Phase III clinical trial testing undergo administering and screening. For example, a very unique and sensitive diabetes drug requires administering and screening the drug over at least 5-7 days of time in the hospital with frequent monitoring/testing and patient medication adherence training with a mobile application. A predictive model was built that can identify which type of patients the drug should be tested on. Target patients were people that were likely to be in the hospital for this duration of time and would not incur significant additional costs for administering this drug to the patient and monitoring.

In order to achieve this goal a regression model was built that could predict the estimated hospitalization time for a patient and use this to select/filter patients for the study.

Expected Hospitalization Time Regression Model: Utilizing a synthetic dataset(denormalized at the line level augmentation) built off of the UCI Diabetes readmission dataset, a regression model was built that predicts the expected days of hospitalization time and then convert this to a binary prediction of whether to include or exclude that patient from the clinical trial.

This project demonstrated the importance of building the right data representation at the encounter level, with appropriate filtering and preprocessing/feature engineering of key medical code sets. This model was also analyzed and interpreted for biases across key demographic groups.

### Dataset
Due to healthcare PHI regulations (HIPAA, HITECH), there are limited number of publicly available datasets and some datasets require training and approval. Therefore, dataset is limited in its representation of some key features such as diagnosis codes which are usually an unordered list in 835s/837s (the HL7 standard interchange formats used for claims and remits).

<a href="https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008">Dataset</a>
Source Code: <a href="https://github.com/kshptl/Patient-Selection-for-Diabetes-Drug-Testing-using-EHR-Data"><i class="large github icon"></i>https://github.com/nathancy/LM-CEW-Automation-</a>


