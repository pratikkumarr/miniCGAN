# MiniCGAN Lab — Generate Handwritten Digits

**Course:** Deep Learning and Generative AI (CS312B)  
**Class:** B.Tech CSE — 5th Semester, Section C

## Team Members

| Name | Roll Number |
|---|---|
| Navya Sharma | 2400290120162 |
| Pratik Kumar | 2400290120187 |
| Prince Rajput | 2400290120190 |

## Project Description

This project trains a **Conditional Generative Adversarial Network (CGAN)** on the MNIST handwritten-digit dataset. The digit label is supplied as a condition to both the generator and discriminator, allowing the generator to create images for a requested digit from **0 to 9**.

## Concepts Implemented

- Generator and discriminator
- Conditional generation using digit labels
- Latent noise vectors
- Binary cross-entropy loss and Adam optimizers
- Adversarial training with gradient updates
- Training-loss visualization and generated-image inspection

## Run in Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `MiniCGAN_Lab_MNIST.ipynb`.
3. For faster training, select **Runtime → Change runtime type → T4 GPU** (optional).
4. Run all cells from top to bottom.
5. View the loss plot and generated digit samples in the notebook.

The MNIST dataset is loaded through TensorFlow/Keras when the notebook runs. No separate dataset download is required.

## Training Configuration

| Parameter | Value |
|---|---:|
| Dataset | MNIST |
| Image size | 28 × 28, grayscale |
| Classes | 10 (digits 0–9) |
| Latent dimension | 100 |
| Batch size | 128 |
| Epochs | 30 |
| Optimizer | Adam |
| Learning rate | 0.0002 |
| Loss | Binary cross-entropy |

## Output Files

After the final notebook cell runs, the trained models are saved in the Colab runtime as:

- `cgan_generator.keras`
- `cgan_discriminator.keras`

Download these files from Colab if they need to be kept after the runtime ends.

## Project File

- `MiniCGAN_Lab_MNIST.ipynb` — complete implementation, training, visualization, and model saving.
