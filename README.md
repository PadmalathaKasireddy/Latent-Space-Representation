# 🔍 Latent Space Representation using Autoencoders (AE) & Variational Autoencoders (VAE)

This project explores how Autoencoders (AE) and Variational Autoencoders (VAE) can be used to learn compressed, meaningful representations of high-dimensional data such as handwritten digits from the MNIST dataset. It includes training both models, visualizing their latent spaces, evaluating reconstruction quality, and performing latent vector arithmetic.

---

## 📁 Contents

- 📌 [Objective](#objective)
- 🧠 [Model Architectures](#model-architectures)
- 📉 [Training and Loss Comparison](#training-and-loss-comparison)
- 📊 [Latent Space Visualization](#latent-space-visualization)
- 🧪 [Latent Vector Arithmetic](#latent-vector-arithmetic)
- 📝 [Key Learnings](#key-learnings)
- 🚀 [Future Work](#future-work)
- 📎 [Presentation](#presentation)
- 👤 [Author](#author)

---

## 🎯 Objective

1. **Build AE and VAE** using PyTorch/Keras and train on MNIST dataset.
2. **Visualize the Latent Space** to see how images are distributed after compression.
3. **Compare Reconstruction Quality** between AE and VAE.
4. **Perform Latent Vector Arithmetic** to demonstrate interpolation and generative capabilities.

---

## 🧠 Model Architectures

### 🔹 Autoencoder (AE)
- **Encoder**: Compresses input image to a lower-dimensional representation.
- **Decoder**: Reconstructs the image from the encoded vector.
- **Loss**: Mean Squared Error (MSE)
- **Activation Functions**: ReLU in hidden layers, Sigmoid in output layer

### 🔹 Variational Autoencoder (VAE)
- **Encoder Outputs**: Mean (μ) and Standard Deviation (σ)
- **Reparameterization Trick**: 
  \[
  z = \mu + \sigma \cdot \epsilon \quad \text{where } \epsilon \sim \mathcal{N}(0, 1)
  \]
- **Loss**: Reconstruction Loss + KL Divergence

---

## 📉 Training and Loss Comparison

- Both AE and VAE models show decreasing loss over epochs.
- AE trains faster and gives sharper reconstructions.
- VAE converges slowly but learns smoother latent representations useful for generation.

---

## 📊 Latent Space Visualization

- **AE**: Latent vectors are often entangled and unstructured.
- **VAE**: Latent vectors exhibit clear clustering of classes.
- **Tools Used**: PCA / t-SNE for 2D projection of high-dimensional latent vectors.

---

## 🧪 Latent Vector Arithmetic

- Performed interpolation between digits, e.g., morphing digit "3" into "8".
- Demonstrates VAE's ability to generate meaningful transitions across latent space.

---

## 📝 Key Learnings

- Latent space acts as a compressed representation where similar data points are close.
- AE is better at compression, VAE is better at generation.
- Visualization tools help understand abstract features learned by the model.

---

## 🚀 Future Work

- Train on more complex datasets (e.g., CIFAR-10).
- Experiment with different latent dimensions and loss functions.
- Explore conditional VAEs or GANs for better generative performance.

---

## 📎 Presentation

The entire project is documented in the following presentation:

📂 **[Google Colab Notebook](https://colab.research.google.com/drive/1raVa0_2TtQY7wO0hku1kk--urz-vJAaa?usp=sharing)**  
📄 **[PPT File](""C:\Users\PADMALATHA\Latent-Space-Representation-using-AE-and-VAE.pptx"")**

---

## 👤 Author

**Padmalatha Kasireddy**  
Department of CSE (AI & ML), GITAMW  
📧 Email: padmalatha3633@gmail.com  
🔗 LinkedIn: *[Add your LinkedIn profile link]*

---

## 🧠 Acknowledgements

Special thanks to **NextHub Technologies Pvt Ltd** for providing mentorship as part of the Generative AI Internship program.

---



