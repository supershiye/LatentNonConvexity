# LatentNonConvexity

This project demonstrates the use of a **Variational Auto-Encoder (VAE)** with a 2-dimensional latent space, combined with a **regressor** to map latent vectors to digit values using the MNIST dataset. The project also visualizes the latent space with regressor contours and highlights the high-density latent region using a data-driven approach.

## Features

1. **Train a Variational Auto-Encoder (VAE):**
   - Encodes MNIST digits into a 2-dimensional latent space.
   - Decodes latent vectors back into digit images.

2. **Train a Regressor:**
   - A 3-layer Multi-Layer Perceptron (MLP) regressor maps latent vectors to digit values.

3. **Visualize Latent Space:**
   - Draws regressor output contours across the latent space.
   - Overlays a high-density latent region using a Gaussian Kernel Density Estimate (KDE).

4. **Highlight Invalid Decodings:**
   - Masks areas of the latent space that lead to invalid decodings.

## Dependencies

The following Python libraries are required:
- `torch`
- `torchvision`
- `matplotlib`
- `scipy`
- `scikit-learn`
- `numpy`

## How to Run

1. Install the required dependencies.
2. Run the script using:
   ```bash
   python main.ipynb
