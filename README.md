
---

# Skin Diseases Classification

This project focuses on classifying skin diseases using machine learning techniques, specifically leveraging a custom Convolutional Neural Network (CNN) and a pre-trained VGG16 model. The aim is to assist individuals and healthcare providers in identifying skin conditions quickly and accurately.

## Problem Definition and Importance

Skin diseases are prevalent health concerns affecting individuals globally. Timely diagnosis and access to dermatological expertise are crucial for effective treatment. This project targets individuals lacking immediate access to dermatologists and those seeking preliminary insights into their skin conditions.

## Solution Overview

### Model Architectures

1. **Custom CNN Architecture**
    - **Flexibility**: Tailored specifically to the skin disease dataset.
    - **Efficiency**: Lightweight and fast, suitable for mobile applications.
    - **Components**:
        - Conv2D Layers: Extract essential features like texture and color variations.
        - MaxPooling: Reduces dimensionality and prevents overfitting.
        - Dense Layers: Consolidates learned features for classification.
        - Dropout: Mitigates overfitting, ensuring better generalization.

2. **Pre-Trained VGG16 Model**
    - **Transfer Learning**: Utilizes pre-trained weights from the ImageNet dataset.
    - **Fine-Tuning**: Adapts to domain-specific patterns while retaining pre-trained knowledge.
    - **High Accuracy**: Strong feature extraction capabilities and robust convolutional layers.
    - **Optimizer**: AdamW optimizer for efficient convergence.

### Comparison and Justification

- **Custom CNN Model**: Ideal for lightweight mobile applications with limited computational resources.
- **VGG16 Model**: Provides higher accuracy and robustness for production environments.

By combining these approaches, the system ensures flexibility, efficiency, and scalability.

## Datasets

1. **Wound**:
    - Wound_dataset
    - Abrasions
    - Bruises
    - Cut
    - Laceration
    - Stab_wound
2. **Bites**:
    - Ants
    - Bed Bugs
    - Chiggers
    - Fleas
    - Mosquitoes
    - Spiders
    - Ticks
3. **Skin**:
    - Healthy Skin

## Data Loading and Processing

The data is loaded into training and testing dataframes, split into validation and test sets, and processed for model training.

## Training and Evaluation

The models are trained using the training dataset and evaluated using validation and test datasets. The performance metrics are recorded and analyzed to fine-tune the models.

## Results

The results demonstrate the effectiveness of using a combination of custom CNN and VGG16 architectures in classifying skin diseases with high accuracy. The detailed performance highlights and visualizations are provided in the notebook.

## Installation and Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/rafalgi/Skin-diseases-classification.git
    ```
2. Navigate to the project directory:
    ```bash
    cd Skin-diseases-classification
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the Jupyter Notebook to train and evaluate the models:
    ```bash
    jupyter notebook Final\ Project.ipynb
    ```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- The pre-trained VGG16 model is sourced from the Keras library.
- The datasets used in this project are publicly available and sourced from various medical image repositories.

---

Feel free to modify this draft as per your specific requirements or additional details you may want to include.
