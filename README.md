# mri-denoising-unet-api
"A deep learning medical imaging API for denoising MRI scans using a U-Net architecture, built with PyTorch and FastAPI."

MRI Denoising & Enhancement API
Specialized Computer Vision Project
This repository features an end-to-end medical imaging system that uses a U-Net Convolutional Neural Network to reconstruct and denoise MRI scans.
🛠 Tech Stack
Deep Learning: PyTorch, MONAI
Backend: FastAPI, Uvicorn
Data Science: NumPy, Nibabel (NIfTI processing), Matplotlib
Environment: Google Colab / Tesla T4 GPU
🧠 The Engineering Approach
Mathematical Core: Implemented Min-Max normalization to stabilize training and prevent checkerboard artifacts.
Data Engineering: Developed a specialized pipeline for 3D NIfTI slice extraction and spatial cropping to $128 \times 128$.
Model: Architected a 5-layer U-Net with skip connections to preserve anatomical integrity during denoising.
MLOps: Wrapped the model in an asynchronous FastAPI service for real-time inference.
📊 Results
Training Time: ~60 seconds (GPU accelerated)
Final Loss (MSE): 0.0002
Performance: Sub-second latency for single-slice processing.
