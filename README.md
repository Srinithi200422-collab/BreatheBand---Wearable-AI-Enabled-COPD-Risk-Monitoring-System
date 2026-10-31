# BreatheBand---Wearable-AI-Enabled-COPD-Risk-Monitoring-System

A wearable prototype designed to explore early COPD risk assessment using physiological signals and lightweight AI.

## About the Project

Chronic Obstructive Pulmonary Disease (COPD) is a progressive lung disease that can affect a person's ability to breathe. Early identification of risk and regular monitoring of respiratory health are important, particularly for people who may have limited access to frequent clinical assessment.

**BreatheBand** is a wearable prototype developed to explore how physiological signals and artificial intelligence can support COPD risk assessment. The device is designed as a chest-strap-based system that collects vital parameters, processes the data using an AI model, and provides an estimated lung-function value and COPD severity category.

The project combines embedded hardware, sensor-based data acquisition, AI-based prediction, and a compact wearable design. The current repository includes the Python implementation, prototype images, sample output images, and a demonstration video.

This is a research and development prototype. It is not a clinically validated diagnostic device and does not replace spirometry or medical evaluation.

## Project Objectives

- Develop a wearable prototype for monitoring selected physiological parameters.
- Acquire SpO₂, heart rate, and respiratory-rate measurements using sensors.
- Use an AI model to estimate FEV₁ percentage predicted and classify COPD severity.
- Explore the integration of AI-based prediction with an embedded wearable system.
- Design a compact, low-cost chest-strap-based prototype for respiratory health monitoring.

## System Overview

The project is organized around the following components:

1. **Physiological data acquisition:** Sensors are used to obtain SpO₂, heart rate, and respiratory-rate information.
2. **Embedded processing:** An ESP32-based controller forms the core of the wearable hardware.
3. **AI-based prediction:** The Python model processes physiological and demographic inputs to estimate FEV₁% predicted and COPD severity.
4. **Output and feedback:** The system presents the estimated values and severity-related output.
5. **Wearable prototype:** The electronics are integrated into a chest-strap-based design.

## Hardware Components

The prototype design includes:

| Component | Purpose |
|---|---|
| ESP32 controller | Main embedded controller |
| MAX30102 | SpO₂ and heart-rate sensing |
| MPU6050 | Respiratory-rate signal acquisition |
| OLED display | Display of measured values and prediction output |
| Push button | User input and device control |
| Li-ion battery | Portable power supply |
| TP4056 module | Battery charging |
| Chest strap and enclosure | Wearable assembly |

The exact hardware configuration may vary between prototype revisions.

## Software and Technologies

- Python
- NumPy and Pandas
- Scikit-learn
- AI model for FEV₁% prediction and COPD severity classification
- Embedded firmware for ESP32-based sensor acquisition

## Repository Contents

```text
BreatheBand/
├── README.md
├── COPD_Model.ipynb
├── media/
│   ├── prototype/
│   │   ├── prototype_01.jpg
│   │   └── ...
│   ├── outputs/
│   │   ├── output_01.png
│   │   └── ...
│   └── demo_video_link.md
├── docs/
│   └── publication.md
└── requirements.txt
```

The main Python file contains the AI-model implementation. The `media/` directory contains prototype photographs, sample outputs, and the demonstration video link.

## Demo

**Working prototype video:** [Watch the demonstration](<ADD_VIDEO_LINK>)

## Prototype Images

The `media/prototype/` directory contains photographs showing the BreatheBand prototype from different views.

## Sample Outputs

The `media/outputs/` directory contains sample outputs generated during model testing and project demonstration.

These outputs illustrate the model's prediction workflow. They should not be interpreted as clinical results or medical diagnoses.

## AI Model and Research Publication

The AI model used in this project is described in the following conference paper:

**“A Lightweight Neural Model for COPD Severity Prediction Suitable for Wearable Deployment”**

Published in the *2026 5th OPJU International Technology Conference (OTCON) on Smart Computing for Innovation and Advancement in Industry 5.0*.

- **Authors:** S. Srinithi, G. Manisha, R. Murugesan, B.B. Dash, U.C. De, and S.S. Patra
- **DOI:** [10.1109/OTCON69332.2026.11629742](https://doi.org/10.1109/OTCON69332.2026.11629742)
- **Paper scope:** AI model for FEV₁% prediction and COPD severity classification

The publication focuses on the AI model. This GitHub repository presents the broader BreatheBand project, including the wearable prototype and its demonstration.

## Limitations

- The prototype is intended for research and demonstration.
- The AI model's performance depends on the data and assumptions used during development.
- Sensor measurements may be affected by motion, placement, and signal quality.
- The system has not been established as a clinically validated COPD screening or diagnostic device.
- Clinical evaluation and comparison with spirometry would be required before any medical use.

## Future Improvements

- Further validation using appropriate real-world physiological data.
- Improved sensor signal quality and respiratory-rate estimation.
- Refinement of embedded inference and wearable power consumption.
- Additional testing across different users and operating conditions.
- Evaluation of usability and reliability in practical settings.

## Authors

- S. Srinithi
- G. Manisha

