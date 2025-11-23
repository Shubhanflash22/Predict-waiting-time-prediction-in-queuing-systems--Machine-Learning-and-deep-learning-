# Waiting Time Prediction in Queuing Systems 🏦⏱️

A machine learning and deep learning project to predict customer waiting times in queuing systems, demonstrated on a banking dataset.

## Table of Contents

* [Project Overview](#project-overview)
* [Dataset](#dataset)
* [Features](#features)
* [Installation](#installation)
* [Usage](#usage)
* [Models](#models)
* [Results](#results)
* [Future Work](#future-work)
* [License](#license)

## Project Overview

This project develops neural network-based models to predict waiting times in queuing systems. The model was trained on bank queue datasets and demonstrated improved accuracy over naive baseline models.

Key components include:

* Training queue-specific neural networks.
* Simulating queuing scenarios for validation.
* Generalizing the approach for multiple industries beyond banking.

## Dataset

* Dataset contains historical queue data from banks, including customer arrival times, service durations, and waiting times.
* Preprocessed for training by normalizing features and removing outliers.
* Although industry-specific, the data structure allows adaptation to other service sectors.

## Features

* **Waiting Time Prediction:** Neural network predicts waiting times for each customer.
* **Queue-Specific Models:** Individual models trained per queue for better accuracy.
* **Simulation Verification:** Validated model predictions using a simulator integrated into a web application.
* **Industry Generalization:** Approach can be applied to different queuing environments.

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/queue-wait-time-prediction.git
cd queue-wait-time-prediction

# Install required Python packages
pip install -r requirements.txt
```

## Usage

1. Prepare queue dataset in CSV format.
2. Run preprocessing script:

```bash
python preprocess_data.py
```

3. Train the neural network model:

```bash
python train_model.py
```

4. Predict waiting times for new customers:

```bash
python predict_waiting_time.py --input new_queue_data.csv
```

## Models

* **Neural Network:** Predicts waiting times based on queue features.
* **Comparison Baselines:** Evaluated against naive models such as mean waiting time predictors.
* **Simulation Verification:** Ensures model predictions align with actual queue dynamics.

## Results

* Achieved a mean absolute error (MAE) of 2.68 minutes, outperforming naive models.
* Queue-specific neural networks demonstrated strong predictive capabilities.
* Successfully verified predictions using simulation in a web application environment.

## Future Work

* Expand to multi-queue and multi-service environments.
* Integrate reinforcement learning for dynamic queue management.
* Apply to other industries such as hospitals, call centers, and retail.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
