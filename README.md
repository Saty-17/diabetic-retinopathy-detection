# Diabetic Retinopathy Detection using VGG19

This project is a deep learning-based approach for detecting **Diabetic Retinopathy** from retinal fundus images. It uses a pre-trained **VGG19** model with transfer learning, implemented in **TensorFlow** and developed in **Jupyter Notebook**. The dataset is sourced from Kaggle, and a simple **frontend interface** is built using HTML and CSS for prediction visualization.

## Overview

Diabetic Retinopathy is one of the leading causes of vision loss. Early detection can help prevent blindness. This model aims to classify the severity of the disease based on retina images.

## Project Structure

```
├── model/
│   └── vgg19_retinopathy_model.h5    # Trained model
├── notebook/
│   └── diabetic_retinopathy.ipynb    # Main Jupyter Notebook
├── static/
│   └── style.css                     # CSS styling
├── templates/
│   └── index.html                    # HTML frontend
├── app.py                            # Flask app (if applicable)
├── README.md
└── requirements.txt
```

## Model

- **Architecture**: VGG19 (pre-trained on ImageNet)
- **Framework**: TensorFlow / Keras
- **Training Details**:
  - Optimizer: Adam
  - Loss: Categorical Crossentropy
  - Data Augmentation: Yes
  - Batch Normalization: Yes

## Dataset

- 📥 Source: [Kaggle - Diabetic Retinopathy Detection](https://www.kaggle.com/c/diabetic-retinopathy-detection)
- 💽 Format: High-resolution retinal images
- 📊 Labels: 5 classes (0: No DR, 1: Mild, 2: Moderate, 3: Severe, 4: Proliferative DR)

## Frontend

- Built with **HTML5** and **CSS3**
- Simple drag-and-drop interface to upload retina images
- Displays model prediction after processing

## How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/diabetic-retinopathy-vgg19.git
   cd diabetic-retinopathy-vgg19
   ```

2. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook or Flask app:
   - Jupyter:
     ```bash
     jupyter notebook
     ```
   - Flask (if applicable):
     ```bash
     python app.py
     ```

## Results

| Metric         | Value     |
|----------------|-----------|
| Accuracy       | 46%       |
| Loss           | ~0.78     |
| Model Used     | VGG19     |

> Note: Results may vary depending on training duration and data preprocessing.

## Future Improvements

- Add Grad-CAM visualization for interpretability
- Optimize model for mobile or web deployment
- Expand dataset for improved generalization

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- [Kaggle Diabetic Retinopathy Dataset](https://www.kaggle.com/c/diabetic-retinopathy-detection)
- [VGG19 Paper](https://arxiv.org/abs/1409.1556)
- TensorFlow & Keras

## Contact

Feel free to reach out via [GitHub Issues](https://github.com/yourusername/diabetic-retinopathy-vgg19/issues) for questions or contributions!
