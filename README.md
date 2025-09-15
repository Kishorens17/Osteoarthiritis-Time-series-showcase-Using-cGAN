# Osteoarthritis Time-Series Visualization using cGAN

## 📌 Overview  
This project implements a **Conditional Generative Adversarial Network (cGAN)** to visualize the **progression of Osteoarthritis (OA)** over time. By learning from real-world medical data, the model generates synthetic yet realistic knee joint images corresponding to different stages and time-points in OA progression. These time-series visualizations support clinicians and researchers in understanding disease patterns and forecasting its progression.

## 🗂 Dataset Used  
We used the publicly available **[Osteoarthritis Initiative (OAI) dataset](https://www.kaggle.com/datasets/jeftaadriel/osteoarthritis-initiative-oai-dataset)**.  

- Contains knee **X-ray images** and related metadata for thousands of patients.  
- Covers **5 stages** of OA severity: from healthy to severely affected.  
- Provides longitudinal (follow-up) data, enabling **time-series analysis** of disease progression.  
- Includes demographic and clinical variables for enriched conditional generation.

## 🛠 Techniques Implemented  
- **Conditional GAN (cGAN)**  
  - Generator conditions on stage/time labels to produce realistic OA images.  
  - Discriminator distinguishes real vs. generated images conditioned on the same labels.  

- **Time-Series Conditioning**  
  - Uses patient follow-up visits as a temporal index to teach the generator how OA appearance evolves.  

- **Image Preprocessing**  
  - Resizing, normalization, and augmentation of X-ray images for stable GAN training.  

- **Training Stability Enhancements**  
  - Applied label smoothing, spectral normalization, and progressive learning rate scheduling to avoid mode collapse.  

- **Visualization**  
  - Generated synthetic OA progression sequences for unseen patients and visualized them as **animated time series**.  

## 🌐 Real-Time Applications  
- **Clinical Decision Support**: Simulate future OA progression for a patient based on current scans and risk factors.  
- **Medical Education & Training**: Provide trainees with diverse, realistic examples of disease stages and transitions.  
- **Data Augmentation for AI Models**: Enhance training datasets for downstream diagnostic models with high-quality synthetic images.  
- **Research on Disease Dynamics**: Explore how OA evolves across different populations, improving preventive and therapeutic strategies.  
