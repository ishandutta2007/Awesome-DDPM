# Awesome-DDPM 🚀

<div align="center">
  <img src="./banner.svg" alt="Awesome DDPM Banner" width="100%" />
  
  <p align="center">
    <a href="https://github.com/ishandutta2007/Awesome-DDPM/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ishandutta2007/Awesome-DDPM?style=for-the-badge&color=gold" /></a>
    <a href="https://github.com/ishandutta2007/Awesome-DDPM/network/members"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ishandutta2007/Awesome-DDPM?style=for-the-badge&color=blue" /></a>
    <a href="https://github.com/ishandutta2007/Awesome-DDPM/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ishandutta2007/Awesome-DDPM?style=for-the-badge&color=red" /></a>
    <a href="https://github.com/ishandutta2007/Awesome-DDPM/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/github/license/ishandutta2007/Awesome-DDPM?style=for-the-badge&color=green" /></a>
    <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow&style=for-the-badge" /></a>
  </p>
  
  <p><b>A curated list of awesome Denoising Diffusion Probabilistic Models (DDPM), papers, and resources.</b></p>
</div>

---

## 📖 Introduction

Denoising Diffusion Probabilistic Models (**DDPMs**) are state-of-the-art generative models 🎨 that construct data by reversing a step-by-step noising process. While the core framework remains the same, the models have evolved into several specialized variants to improve speed, efficiency, and conditioning for specific generation tasks.

<div align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNHJqZ3R5Mnd6Mnd6Mnd6Mnd6Mnd6Mnd6Mnd6Mnd6Mnd6Mnd6Mnd6JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZCZjdD1n/3o7TKVUn7iM8FMEU24/giphy.gif" alt="Diffusion Process Visualization" width="400" />
</div>

## 🛠️ Core Types and Variants

| Model | Description | Year | Paper Link | More Details |
| :--- | :--- | :--- | :--- | :--- |
| **Standard DDPMs (Markovian)** | The foundational model that progressively adds Gaussian noise to an image in a forward chain, and then trains a neural network (usually a U-Net) to reverse this process over hundreds or thousands of iterative steps. | 2020 | [arXiv:2006.11239](https://arxiv.org/abs/2006.11239) | [Detailed Info](./docs/standard-ddpm.md) |

| Model | Description | Year | Paper Link | More Details |
| :--- | :--- | :--- | :--- | :--- |
| **Latent Diffusion Models (LDMs)** | Instead of processing full-sized images directly, LDMs compress the data into a lower-dimensional latent space to perform the diffusion process. This significantly reduces computational costs and powers major commercial generators like Stable Diffusion. | 2021 | [arXiv:2112.10752](https://arxiv.org/abs/2112.10752) | [Detailed Info](./docs/latent-diffusion.md) |

| Model | Description | Year | Paper Link | More Details |
| :--- | :--- | :--- | :--- | :--- |
| **Denoising Diffusion Implicit Models (DDIM)** | DDIM modifies the reverse process to make it non-Markovian. This allows the model to produce high-quality images much faster than standard DDPMs by skipping intermediate steps without having to retrain the underlying model. | 2020 | [arXiv:2010.02502](https://arxiv.org/abs/2010.02502) | [Detailed Info](./docs/ddim.md) |

| Model | Description | Year | Paper Link | More Details |
| :--- | :--- | :--- | :--- | :--- |
| **Guided Diffusion** | Enhances control over the generated output by using either classifier guidance or classifier-free guidance. This allows the model to align its outputs with specific conditions, such as text prompts (e.g., DALL·E 2) or class labels. | 2021 | [arXiv:2105.05233](https://arxiv.org/abs/2105.05233) | [Detailed Info](./docs/guided-diffusion.md) |

| Model | Description | Year | Paper Link | More Details |
| :--- | :--- | :--- | :--- | :--- |
| **Score-Based Generative Models (SGMs) / SDEs** | A mathematically equivalent framework that treats the diffusion process as a continuous-time Stochastic Differential Equation (SDE) rather than discrete steps. This approach excels at generating continuous data and allows for exact likelihood computation. | 2020 | [arXiv:2011.13456](https://arxiv.org/abs/2011.13456) | [Detailed Info](./docs/score-based-sde.md) |

## 🚀 Common Use Cases

*   **Text-to-Image Generation 📝➡️🖼️:** Creating completely new, high-quality images from text descriptions.
*   **Image-to-Image / Inpainting 🖼️➡️🎨:** Filling in missing or masked parts of an existing image.
*   **Super-Resolution 🔍➡️✨:** Taking a blurry or low-resolution image and upscaling it to a sharp, high-definition version.

---

## 🏷️ SEO & Metadata
<!--
Keywords: DDPM, Denoising Diffusion Probabilistic Models, Generative AI, Machine Learning, Stable Diffusion, LDM, DDIM, Guided Diffusion, Score-Based Models, AI Papers, Awesome List
Description: A curated collection of the best resources, papers, and implementations of Denoising Diffusion Probabilistic Models (DDPM).
-->

## 📈 Star History
<div align="center">
   <a href="https://www.star-history.com/#ishandutta2007/Awesome-DDPM&Date">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/Awesome-DDPM&type=Date&theme=dark" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/Awesome-DDPM&type=Date" />
      <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/Awesome-DDPM&type=Date" />
    </picture>
   </a>
</div>
