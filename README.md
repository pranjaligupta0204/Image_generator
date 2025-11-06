# AI Image Generator

This project is an **AI-powered image generation web app** built using **Stable Diffusion**, **PyTorch**, and **Gradio**.  
It allows users to enter a text prompt and instantly generate a high-quality, AI-generated image.  
The model runs on GPU for fast inference and supports customization like creativity level and quality steps.

---

## Overview

The **AI Image Generator** provides an intuitive web interface where users can:
- Enter a **text prompt** describing the desired image.
- Optionally add a **negative prompt** to exclude unwanted details.
- Adjust **creativity** and **quality settings** using sliders.
- Instantly view and download the generated image.
- Automatically log generated prompts and save images locally.

---

## Key Features

- **Text-to-Image Generation:** Creates realistic or artistic images from text prompts.
- **Negative Prompt Support:** Lets users exclude elements (e.g., “blurry”, “low quality”).
- **Customizable Outputs:** Adjust *guidance scale* and *inference steps* for creative control.
- **Real-Time Preview:** Displays generated images directly in the Gradio interface.
- **Auto-Save & Logging:** Saves images with timestamps and logs all prompts to a text file.
- **GPU Optimization:** Utilizes CUDA for faster model inference.
- **Clean & Interactive UI:** Built using Gradio Blocks layout.

---

## Model Information

- **Base Model:** [`runwayml/stable-diffusion-v1-5`](https://huggingface.co/runwayml/stable-diffusion-v1-5)  
- **Framework:** [Diffusers](https://github.com/huggingface/diffusers)  
- **Inference Device:** GPU (`torch.cuda`)

---

## Tech Stack & Libraries Used

### **Core Frameworks**
- `torch` – PyTorch for model execution and GPU acceleration  
- `diffusers` – Hugging Face library for Stable Diffusion pipeline  
- `gradio` – Interactive web UI for prompt input and image display  

### **Supporting Libraries**
- `PIL` – Image handling and saving (via `Pillow`)  
- `os` – File system operations for saving images  
- `datetime` – Timestamps for filenames and logs  
- `gc` – Manual garbage collection for GPU memory cleanup  
- `logging` – Error handling and process tracking  

---
