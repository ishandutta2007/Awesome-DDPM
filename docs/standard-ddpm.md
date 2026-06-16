# Standard DDPMs (Markovian)

Denoising Diffusion Probabilistic Models (DDPMs) are a class of generative models that learn to produce data by reversing a progressive noising process.

## 🔬 Core Mechanism
The process involves two main chains:
1. **Forward Process (Diffusion):** Gradually adds Gaussian noise to the data until it becomes pure noise.
2. **Reverse Process (Denoising):** A neural network learns to remove noise step-by-step to recover the original data.

## 📊 Process Diagram
<div align="center">
<svg width="600" height="200" viewBox="0 0 600 200" xmlns="http://www.w3.org/2000/svg">
  <!-- Forward Process -->
  <rect x="50" y="70" width="80" height="60" rx="10" fill="#4CAF50" />
  <text x="90" y="105" text-anchor="middle" fill="white" font-family="Arial" font-size="12">Data (x₀)</text>
  
  <path d="M 140 100 L 190 100" stroke="#555" stroke-width="2" marker-end="url(#arrowhead)" />
  
  <rect x="200" y="70" width="80" height="60" rx="10" fill="#8BC34A" />
  <text x="240" y="105" text-anchor="middle" fill="white" font-family="Arial" font-size="12">Noisy (xₜ)</text>
  
  <path d="M 290 100 L 340 100" stroke="#555" stroke-width="2" marker-end="url(#arrowhead)" />
  
  <rect x="350" y="70" width="80" height="60" rx="10" fill="#CDDC39" />
  <text x="390" y="105" text-anchor="middle" fill="white" font-family="Arial" font-size="12">Noise (xₜ)</text>
  
  <!-- Reverse Labels -->
  <path d="M 340 130 L 290 130" stroke="#F44336" stroke-width="2" marker-end="url(#arrowhead)" />
  <path d="M 190 130 L 140 130" stroke="#F44336" stroke-width="2" marker-end="url(#arrowhead)" />
  
  <text x="240" y="160" text-anchor="middle" fill="#F44336" font-family="Arial" font-size="10">Reverse (Learning)</text>
  <text x="240" y="40" text-anchor="middle" fill="#4CAF50" font-family="Arial" font-size="10">Forward (Fixed)</text>
  
  <defs>
    <marker id="arrowhead" markerWidth="10" markerHeight="7" refX="0" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" />
    </marker>
  </defs>
</svg>
</div>

## 📄 Key Papers
- **Denoising Diffusion Probabilistic Models** (Ho et al., 2020): [Link](https://arxiv.org/abs/2006.11239)

[⬅ Back to README](../README.md)
