# Score-Based Generative Models (SGMs) / SDEs

Score-based models unify diffusion into a continuous-time framework using Stochastic Differential Equations (SDEs).

## 🔬 Core Mechanism
Instead of discrete steps, the noise process is modeled as a continuous SDE. The reverse process (generation) is then solved as a reverse-time SDE, which involves estimating the "score function" (gradient of the log-density).

## 📊 Process Diagram
<div align="center">
<svg width="600" height="200" viewBox="0 0 600 200" xmlns="http://www.w3.org/2000/svg">
  <path d="M 50 150 Q 150 50 300 100 T 550 50" stroke="#607D8B" fill="transparent" stroke-width="3" />
  <text x="300" y="130" text-anchor="middle" font-family="Arial" font-size="12" fill="#37474F">Continuous SDE Path</text>
  
  <circle cx="50" cy="150" r="5" fill="#263238" />
  <text x="50" y="170" text-anchor="middle" font-family="Arial" font-size="10">x₀</text>
  
  <circle cx="550" cy="50" r="5" fill="#263238" />
  <text x="550" y="40" text-anchor="middle" font-family="Arial" font-size="10">x_T</text>
  
  <path d="M 300 100 L 330 70" stroke="#FF5252" stroke-width="2" marker-end="url(#arrowhead)" />
  <text x="350" y="80" font-family="Arial" font-size="10" fill="#FF5252">Score ∇ log p(x)</text>

  <defs>
    <marker id="arrowhead" markerWidth="10" markerHeight="7" refX="0" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" />
    </marker>
  </defs>
</svg>
</div>

## 📄 Key Papers
- **Score-Based Generative Modeling through Stochastic Differential Equations** (Song et al., 2020): [Link](https://arxiv.org/abs/2011.13456)

[⬅ Back to README](../README.md)
