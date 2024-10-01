# ScenARy: Scene Awareness for Augmented Reality Applications in Assembly Systems

## Key Features

- **Semantic Scene Understanding**: ScenARy introduces context-awareness by recognizing different assembly workstations and dynamically adapting AR content for non-sequential workflows.
- **AR-Based Work Instructions**: The model helps deliver AR instructions that change based on the scene, improving usability in multi-workstation processes such as inspections or maintenance.
- **Egocentric Scene Classification**: Using a custom dataset of factory workplaces, the deep learning model classifies scenes in real-time from AR video streams, providing context-sensitive instructions.
- **Microsoft HoloLens Deployment**: The model is deployed on the Microsoft HoloLens, allowing field operators to receive dynamic instructions as they move between workstations.


## Directory Structure
```
ScenARy-FactoryWorkplaces/
│
├── dataset/                    # Contains the Factory Workplaces dataset used for training the model
│   ├── images/                 # Example images of different manufacturing stations
│   └── labels/                 # Corresponding labels for scene categories
│
├── models/                     # Trained deep learning models for scene classification
│   └── hololens_model          # Model deployed on the Microsoft HoloLens
│
├── src/                        # Source code for model training, evaluation, and deployment
│   ├── train.py                # Script for training the scene classification model
│   ├── evaluate.py             # Model evaluation and performance testing
│   └── deployment/             # Scripts for deploying the model on HoloLens
│       └── hololens_app.py     # HoloLens-specific deployment script
│
├── results/                    # Model performance results and experiments
│   └── accuracy_metrics.csv    # Classification accuracy and other evaluation metrics
│
├── LICENSE                     # License information (CC BY-NC-ND 4.0)
├── README.md                   # Readme file (this file)
└── requirements.txt            # List of dependencies and libraries
```

## Dataset

The **Factory Workplaces** dataset contains six categories of assembly workstations scraped from the internet. The dataset is used to fine-tune a deep learning model for scene classification and can be accessed [here](https://github.com/celairion/ScenARy-FactoryWorkplaces).

## Model

The model is built using deep learning techniques for image classification, fine-tuned to classify various assembly stations. It is designed to run on AR devices such as the Microsoft HoloLens, facilitating real-time scene understanding in complex manufacturing environments.

### Training the Model

To train the model, use the `train.py` script:


## Dependencies

To install the required dependencies, run:

```bash
pip install -r requirements.txt
```

## Citation

If you use the dataset or code, please cite the following paper:

```objectivec
will be updated
```

## Contributions

Contributions are welcome! Feel free to fork the repository, create a new branch, and submit a pull request with your improvements.

## Contact

For any questions or inquiries, please open an issue on this repository or contact the authors at [andreas.steiner@tuwien.ac.at](mailto:andreas.steiner@tuwien.ac.at).
```
