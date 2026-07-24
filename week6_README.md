# Autoencoder for Image Denoising using MNIST

## Project Overview

This project demonstrates how to build a Deep Learning Autoencoder capable of removing noise from handwritten digit images using the MNIST dataset. The model learns to reconstruct clean images from noisy inputs by compressing the image into a lower-dimensional latent representation and then decoding it back to its original form.

---

## Objective

- Load the MNIST handwritten digit dataset.
- Add Gaussian noise to the images.
- Build an Autoencoder using TensorFlow/Keras.
- Train the model to reconstruct clean images.
- Compare Original, Noisy, and Denoised images.
- Save the trained model.

---

## Dataset

Dataset Used:
- MNIST Handwritten Digits Dataset

Number of Images:
- Training Images: 60,000
- Testing Images: 10,000

Image Size:
- 28 × 28 pixels (Grayscale)

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Google Colab / Jupyter Notebook

---

## Project Workflow

1. Load the MNIST dataset.
2. Normalize pixel values.
3. Flatten images into vectors.
4. Add Gaussian noise.
5. Build the Autoencoder.
6. Train the model.
7. Predict denoised images.
8. Visualize results.
9. Save the trained model.

---

## Autoencoder Architecture

### Encoder

- Input Layer (784 neurons)
- Dense Layer (128 neurons, ReLU)
- Dense Layer (64 neurons, ReLU)
- Dense Layer (32 neurons, ReLU)

### Decoder

- Dense Layer (64 neurons, ReLU)
- Dense Layer (128 neurons, ReLU)
- Output Layer (784 neurons, Sigmoid)

---

## Model Compilation

- Optimizer: Adam
- Loss Function: Binary Crossentropy

---

## Training Configuration

- Epochs: 20
- Batch Size: 256
- Validation Dataset: MNIST Test Set

---

## Results

The trained Autoencoder successfully removes most of the artificial Gaussian noise from handwritten digit images.

The output visualization contains:

- Original Images
- Noisy Images
- Reconstructed (Denoised) Images

The reconstructed images closely resemble the original handwritten digits.

---

## Folder Structure

```
MNIST-Autoencoder/
│
├── Autoencoder_MNIST.ipynb
├── mnist_autoencoder.h5
├── README.md
└── requirements.txt
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/MNIST-Autoencoder.git
```

Move into the project directory:

```bash
cd MNIST-Autoencoder
```

Install the required packages:

```bash
pip install -r requirements.txt
```

---

## Run the Project

Launch Jupyter Notebook or Google Colab and execute all notebook cells in order.

The notebook will:

- Load the dataset
- Train the Autoencoder
- Display denoising results
- Save the trained model

---

## Output

The project generates:

- Training Loss Graph
- Validation Loss Graph
- Original Images
- Noisy Images
- Denoised Images
- Trained Model (`mnist_autoencoder.h5`)

---

## Future Improvements

- Convolutional Autoencoder
- Variational Autoencoder (VAE)
- Color Image Denoising
- CIFAR-10 Image Denoising
- Real-world Noise Removal

---

## Requirements

- Python 3.9+
- TensorFlow
- NumPy
- Matplotlib

Install all dependencies using:

```bash
pip install tensorflow numpy matplotlib
```

---

## Conclusion

This project demonstrates the effectiveness of Autoencoders for image denoising. By learning compact latent representations, the model reconstructs clean handwritten digit images from noisy inputs with good accuracy. It serves as a foundation for more advanced image restoration and representation learning tasks.

---

