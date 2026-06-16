# Latent Diffusion Models (LDMs)

Latent Diffusion Models (LDMs) perform the diffusion process in a compressed latent space rather than the high-dimensional pixel space.

## 🔬 Core Mechanism
1. **Autoencoder (VAE):** Compresses images into a latent representation.
2. **Latent Diffusion:** Applies the denoising process within this compressed space.
3. **Conditioning:** Incorporates external inputs like text via cross-attention mechanisms.

## 📊 Process Diagram
<div align="center">
<svg width="600" height="250" viewBox="0 0 600 250" xmlns="http://www.w3.org/2000/svg">
  <!-- Image Space -->
  <rect x="50" y="100" width="100" height="80" rx="5" fill="#2196F3" stroke="#0D47A1" stroke-width="2" />
  <text x="100" y="145" text-anchor="middle" fill="white" font-family="Arial" font-size="12">Pixel Space</text>
  
  <!-- Encoder -->
  <path d="M 160 140 L 220 140" stroke="#333" stroke-width="2" marker-end="url(#arrowhead)" />
  <text x="190" y="130" text-anchor="middle" font-family="Arial" font-size="10">Encoder</text>
  
  <!-- Latent Space -->
  <rect x="230" y="80" width="140" height="120" rx="10" fill="#BBDEFB" stroke="#2196F3" stroke-dasharray="5,5" />
  <text x="300" y="145" text-anchor="middle" fill="#0D47A1" font-family="Arial" font-weight="bold">Latent Space (Z)</text>
  
  <!-- Diffusion in Latent -->
  <circle cx="300" cy="110" r="15" fill="#FFC107" />
  <text x="300" y="115" text-anchor="middle" font-family="Arial" font-size="8">Diffusion</text>
  
  <!-- Decoder -->
  <path d="M 380 140 L 440 140" stroke="#333" stroke-width="2" marker-end="url(#arrowhead)" />
  <text x="410" y="130" text-anchor="middle" font-family="Arial" font-size="10">Decoder</text>
  
  <!-- Output -->
  <rect x="450" y="100" width="100" height="80" rx="5" fill="#2196F3" stroke="#0D47A1" stroke-width="2" />
  <text x="500" y="145" text-anchor="middle" fill="white" font-family="Arial" font-size="12">Generated Image</text>

  <defs>
    <marker id="arrowhead" markerWidth="10" markerHeight="7" refX="0" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" />
    </marker>
  </defs>
</svg>
</div>

## 📄 Key Papers
- **High-Resolution Image Synthesis with Latent Diffusion Models** (Rombach et al., 2021): [Link](https://arxiv.org/abs/2112.10752)

[⬅ Back to README](../README.md)
