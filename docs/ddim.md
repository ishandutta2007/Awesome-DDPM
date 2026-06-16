# Denoising Diffusion Implicit Models (DDIM)

DDIMs introduce a non-Markovian forward process that allows for faster sampling without retraining.

## 🔬 Core Mechanism
Standard DDPMs require many steps because each step depends only on the previous one (Markovian). DDIM breaks this by allowing the next step to depend on both the current step and the original estimate, enabling "skipping" steps during inference.

## 📊 Process Diagram
<div align="center">
<svg width="600" height="200" viewBox="0 0 600 200" xmlns="http://www.w3.org/2000/svg">
  <rect x="50" y="70" width="80" height="60" rx="10" fill="#9C27B0" />
  <text x="90" y="105" text-anchor="middle" fill="white" font-family="Arial" font-size="12">xₜ</text>
  
  <path d="M 140 100 L 250 100" stroke="#555" stroke-width="2" marker-end="url(#arrowhead)" />
  <text x="195" y="90" text-anchor="middle" font-family="Arial" font-size="10">Skip Steps (Fast)</text>
  
  <rect x="260" y="70" width="80" height="60" rx="10" fill="#E1BEE7" />
  <text x="300" y="105" text-anchor="middle" fill="#4A148C" font-family="Arial" font-size="12">xₜ₋ₖ</text>

  <path d="M 350 100 L 460 100" stroke="#555" stroke-width="2" marker-end="url(#arrowhead)" />
  
  <rect x="470" y="70" width="80" height="60" rx="10" fill="#4A148C" />
  <text x="510" y="105" text-anchor="middle" fill="white" font-family="Arial" font-size="12">x₀</text>

  <defs>
    <marker id="arrowhead" markerWidth="10" markerHeight="7" refX="0" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" />
    </marker>
  </defs>
</svg>
</div>

## 📄 Key Papers
- **Denoising Diffusion Implicit Models** (Song et al., 2020): [Link](https://arxiv.org/abs/2010.02502)

[⬅ Back to README](../README.md)
