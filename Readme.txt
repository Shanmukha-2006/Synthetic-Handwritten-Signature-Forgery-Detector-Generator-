# Synthetic Handwritten Signature Forgery Detector & Generator using CycleGAN

## Project Overview

This project uses Deep Learning and Generative AI techniques to generate synthetic handwritten signature samples and detect forged signatures.

It combines a **CycleGAN (Cycle-Consistent Generative Adversarial Network)** for synthetic image generation with a **Convolutional Neural Network (CNN)** for signature classification.

The project is developed using Python and Google Colab.

## Objectives

- Generate synthetic handwritten signature samples using CycleGAN.
- Classify handwritten signatures as genuine or forged.
- Apply deep learning techniques to image generation and classification.
- Evaluate the performance of the trained CNN model.

## Technologies Used

- Python
- Google Colab
- PyTorch
- OpenCV
- NumPy
- Scikit-learn
- CycleGAN
- Convolutional Neural Network (CNN)

## Dataset

**Dataset:** [Handwritten Signatures – Kaggle](https://www.kaggle.com/datasets/divyanshrai/handwritten-signatures)

The dataset contains two categories:

- Genuine signatures: 1,320 images
- Forged signatures: 1,320 images
- Total: 2,640 images

Images are resized to 128 × 128 pixels and normalized before training.

## Project Workflow

### Step 1: Dataset Preprocessing
- Upload and extract the signature dataset.
- Separate genuine and forged signature images.
- Convert images into grayscale.
- Resize images to 128 × 128 pixels.
- Normalize pixel values.

### Step 2: CycleGAN Training
- Build generator and discriminator networks.
- Train CycleGAN to learn transformations between genuine and forged image domains.
- Generate synthetic research samples.

### Step 3: CNN Forgery Detection
- Prepare the image classification dataset.
- Build a CNN model.
- Train the model to classify signatures into genuine and forged categories.

### Step 4: Evaluation and Model Saving
- Evaluate the CNN using test data.
- Calculate accuracy and classification metrics.
- Save the trained generator and detector models.

## Model Architecture

**CycleGAN**
- Generator A → B
- Generator B → A
- Discriminator A
- Discriminator B

**CNN Detector**
- Convolutional layers
- ReLU activation
- Max pooling
- Dropout
- Fully connected layers
- Output classes: Genuine and Forged

## How to Run

1. Open [Google Colab](https://colab.research.google.com/).
2. Select GPU runtime if available.
3. Upload the Kaggle dataset ZIP file.
4. Run the four code cells sequentially.
5. Evaluate the trained detector.
6. Download the saved model ZIP file.

## Output

- Synthetic signature research samples.
- Genuine or forged classification predictions.
- Model evaluation metrics.
- Saved CycleGAN and CNN model weights.

## Future Enhancements

- Improve CycleGAN image generation quality.
- Use writer-independent train/test splitting.
- Increase training epochs and optimize model architecture.
- Develop a Streamlit web application for signature image testing.
- Explore Siamese networks for writer-specific signature verification.

## Disclaimer

This project is developed for educational and research purposes. Synthetic images are generated for experimentation and should not be used to imitate real individuals' signatures. The CNN provides basic genuine/forged image classification and is not a validated real-world signature verification system.

## Author

**DEVALAMKATI SHANMUKHA**

GitHub: https://github.com/Shanmukha-2006
