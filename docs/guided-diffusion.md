# Guided Diffusion

Guided Diffusion techniques allow for better control over the generative process by biasing the reverse steps towards specific classes or text prompts.

## 🔬 Core Mechanism
1. **Classifier Guidance:** Uses a separate classifier to guide the diffusion towards a label.
2. **Classifier-Free Guidance:** Learns both conditional and unconditional distributions simultaneously, avoiding the need for a separate classifier.

## 📊 Process Diagram
<div align="center">
<svg width="600" height="200" viewBox="0 0 600 200" xmlns="http://www.w3.org/2000/svg">
  <rect x="250" y="70" width="100" height="60" rx="10" fill="#FF5722" />
  <text x="300" y="105" text-anchor="middle" fill="white" font-family="Arial" font-size="12">U-Net Model</text>
  
  <path d="M 300 30 L 300 60" stroke="#333" stroke-width="2" marker-end="url(#arrowhead)" />
  <text x="300" y="20" text-anchor="middle" font-family="Arial" font-size="10" fill="#E64A19">Condition (Text/Label)</text>
  
  <path d="M 240 100 L 200 100" stroke="#333" stroke-width="2" />
  <path d="M 360 100 L 400 100" stroke="#333" stroke-width="2" />
  
  <circle cx="300" cy="160" r="20" fill="#FFCCBC" />
  <text x="300" y="165" text-anchor="middle" font-family="Arial" font-size="8">Guidance Scale</text>
  
  <defs>
    <marker id="arrowhead" markerWidth="10" markerHeight="7" refX="0" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" />
    </marker>
  </defs>
</svg>
</div>

## 📄 Key Papers
- **Diffusion Models Beat GANs on Image Synthesis** (Dhariwal & Nichol, 2021): [Link](https://arxiv.org/abs/2105.05233)

[⬅ Back to README](../README.md)
