# 🖼️ Automated Photorealistic Image Generation Pipeline  

🚀 A high-resolution **2048x2048 text-to-image generation pipeline** optimized for **photorealism, steerability, and efficiency**.  
Utilizes **Stable Diffusion**, fine-tuned on **FFHQ** (for realistic faces) and **Flickr8k** (for diverse backgrounds & human scenes).  

## ✨ Features  
✔️ **Photorealistic Human Image Generation** – Fine-tuned for sharp & realistic faces  
✔️ **Multi-Dataset Training** – FFHQ (faces), Flickr8k (scenes), with optimized dataset selection  
✔️ **Efficient Fine-Tuning** – Adaptive chunking, metadata filtering, and prompt steerability  
✔️ **Post-Processing** – Upscaling (OpenCV INTER_CUBIC) for high-quality 2048x2048 images  
✔️ **Optimized for Performance** – Balances quality & computational efficiency  

## 📂 Datasets Used  
- **FFHQ (Flickr-Faces-HQ)** – 70K high-resolution human face images  
- **Flickr8k** – 8K images with detailed captions for scene generation  
- **(Excluded) COCO & DeepFashion** – Tested but led to disfigured images  

## 🏗️ Model & Training Details  
- **Base Model:** `CompVis/stable-diffusion-v1-2`  
- **Fine-Tuning:**  
  - Step 1: **FFHQ** – Enhances human face realism  
  - Step 2: **Flickr8k** – Improves full-body realism & scene diversity  
- **Architecture:**  
  - **Stable Diffusion (Latent Diffusion Model)**
  - **UNet + CLIP Cross-Attention**  
  - **Guidance Scale Optimization (e.g., 7.5 for better adherence to text prompts)**  


