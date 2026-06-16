# Awesome-DDPM
## Denoising Diffusion Probabilistic Models (DDPMs)

Denoising Diffusion Probabilistic Models (DDPMs) are generative models that construct data by reversing a step-by-step noising process. While the core framework remains the same, the models have evolved into several specialized variants to improve speed, efficiency, and conditioning for specific generation tasks.

## Core Types and Variants

* **Standard DDPMs (Markovian):** The foundational model introduced in [2006.11239 on arXiv](https://arxiv.org). It progressively adds Gaussian noise to an image in a forward chain, and then trains a neural network (usually a U-Net) to reverse this process over hundreds or thousands of iterative steps.
* **Latent Diffusion Models (LDMs):** Instead of processing full-sized images directly, LDMs compress the data into a lower-dimensional latent space to perform the diffusion process. This significantly reduces computational costs and powers major commercial generators like [Stable Diffusion](https://arizona.edu).
* **Denoising Diffusion Implicit Models (DDIM):** DDIM modifies the reverse process to make it non-Markovian. This allows the model to produce high-quality images much faster than standard DDPMs by skipping intermediate steps without having to retrain the underlying model.
* **Guided Diffusion:** Enhances control over the generated output by using either **classifier guidance** or **classifier-free guidance**. This allows the model to align its outputs with specific conditions, such as text prompts (e.g., [DALL·E 2](https://arizona.edu)) or class labels. 
* **Score-Based Generative Models (SGMs) / SDEs:** A mathematically equivalent framework that treats the diffusion process as a continuous-time Stochastic Differential Equation (SDE) rather than discrete steps. This approach excels at generating continuous data and allows for exact likelihood computation.

## Common Use Cases

* **Text-to-Image Generation:** Creating completely new, high-quality images from text descriptions.
* **Image-to-Image / Inpainting:** Filling in missing or masked parts of an existing image.
* **Super-Resolution:** Taking a blurry or low-resolution image and upscaling it to a sharp, high-definition version.
