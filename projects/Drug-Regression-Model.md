---
layout: project
type: project
image: images/CEW1.JPG
title: Regression Model to Predict Patient Estimated Hospitalization Time
permalink: projects/Drug-Regression-Model
date: 2020
labels:
  - Python
  - Clinical Data
  - Regression Model
Summary: Built a machine learning model to identify diabetes patients that are likely to be treated with a client drug, thereby ensuring effective reach out of the medical representatives to the corresponding physicians.
---
<div class="ui small rounded images">
  <img class="ui image" src="../images/CEW1.JPG">
  <img class="ui image" src="../images/CEW5.JPG">
  <img class="ui image" src="../images/CEW2.JPG">
  <img class="ui image" src="../images/CEW4.JPG">
</div>

### Project Overview
Drugs that are ready for Phase III clinical trial testing undergo administering and screening. For example, a very unique and sensitive diabetes drug requires administering and screening the drug over at least 5-7 days of time in the hospital with frequent monitoring/testing and patient medication adherence training with a mobile application. A predictive model was built that can identify which type of patients the drug should be tested on. Target patients were people that were likely to be in the hospital for this duration of time and would not incur significant additional costs for administering this drug to the patient and monitoring.

In order to achieve this goal a regression model was built that could predict the estimated hospitalization time for a patient and use this to select/filter patients for the study.

Expected Hospitalization Time Regression Model: Utilizing a synthetic dataset(denormalized at the line level augmentation) built off of the UCI Diabetes readmission dataset, a regression model was built that predicts the expected days of hospitalization time and then convert this to a binary prediction of whether to include or exclude that patient from the clinical trial.

This project demonstrated the importance of building the right data representation at the encounter level, with appropriate filtering and preprocessing/feature engineering of key medical code sets. This model was also analyzed and interpreted for biases across key demographic groups.

### Dataset
Due to healthcare PHI regulations (HIPAA, HITECH), there are limited number of publicly available datasets and some datasets require training and approval. Therefore, dataset is limited in its representation of some key features such as diagnosis codes which are usually an unordered list in 835s/837s (the HL7 standard interchange formats used for claims and remits).

<a href="https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008">Dataset<\a>
Source Code: <a href="https://github.com/kshptl/Patient-Selection-for-Diabetes-Drug-Testing-using-EHR-Data"><i class="large github icon"></i>https://github.com/nathancy/LM-CEW-Automation-</a>

### Project Overview
Continuous electrowetting (CEW) is an electromechanical response that can be used to alter the surface tension of liquid-metal droplets through the application of an electric potential. Galinstan, a liquid metal is injected into an electrolyte-filled channel and manually actuated. Although general control of liquid-metal slug locations has been demonstrated, pinpoint accuracy and automation has yet to be proven. Based on results from initial prototypes, this implementation demonstrates a CEW automation design concept to enable accurate positional control by utilizing a microcontroller and positional feedback sensors to directly improve liquid-metal device testing.

<img class="ui fluid image" src="../images/CEW3.JPG">

### Implementation
Continuous electrowetting automation is implemented using an [Arduino Mega](https://www.arduino.cc/en/Main/arduinoBoardMega2560) microcontroller, a open-source electronics platform, the [Agilent 33220A](http://www.keysight.com/en/pd-127539-pn-33220A/function-arbitrary-waveform-generator-20-mhz?cc=US&lc=eng) waveform generator, and home-made feedback displacement sensors made with [Duroid](http://www.rogerscorp.com/acs/producttypes/6/RT-duroid-Laminates.aspx) and resistors. Over a semester, firmware was developed which utilized feedback displacement sensors and the Arduino serial monitor to implement the process of CEW where the user is able to specify a desired position in the fluidic channel. 

### Learning Outcomes
In this project, I gained experience working with an Arduino microcontroller which included its programming platform and serial interface, C++ for programming the functional abilities of the application, and working with the [CapacitiveSensor Library](https://github.com/PaulStoffregen/CapacitiveSensor) for handling the proximity sensing of the capacitive displacement sensors.
 
Source Code: <a href="https://github.com/nathancy/LM-CEW-Automation-"><i class="large github icon"></i>https://github.com/nathancy/LM-CEW-Automation-</a>


