🛰️ SVAM-AI Mapper
AI-Driven Geospatial Feature Extraction from SVAMITVA Drone Orthophotos

🚀 Developed for the MoPR AI/ML Geospatial Intelligence Hackathon — Problem Statement 1
🤝 In collaboration with Geo-Intel Lab, IIT Tirupati Navavishkar I-Hub Foundation (IITTNiF)

🌍 Overview

SVAM-AiMapper is a modular, end-to-end deep learning pipeline designed to automatically extract key geospatial features from high-resolution SVAMITVA drone orthophotos.

💡 It transforms raw drone imagery into GIS-ready, georeferenced outputs for scalable rural land mapping across India — fully deployable on Google Colaboratory without requiring local GPU infrastructure.

⚙️ What It Does
🏗️ Building Detection
SegFormer-B3 + UNet++ (EfficientNet-B4) ensemble
📊 Achieves 81.9% IoU
Extracts precise building footprints
💧 Water Body Segmentation
Dual-branch MIT-B3 UNet + UNet++ fusion
📊 Achieves 78.9% IoU
Detects ponds, lakes, and small rural water structures
🛣️ Road Extraction
UNet++ + SegFormer-B3
Uses topology-preserving skeleton loss
📊 Achieves 60.3% IoU
Ensures connectivity-aware road mapping
🏠 Roof Type Classification
EfficientNet-B5 classifier
📊 Achieves 96.1% Accuracy
Classifies:
Pucca
Semi-pucca
Kachha
🔥 Key Highlights

✨ Ultra-Large Image Handling

Tile-based windowed inference
Supports orthophotos up to 160,000 × 176,000 pixels
Runs smoothly on Colab T4 GPU

💾 Checkpoint Resilience

Per-village Google Drive checkpointing
Training resumes after session disconnects

📦 GIS-Ready Outputs

Export formats:
GeoJSON
GeoPackage (.gpkg)
CSV
Directly importable into QGIS (no post-processing needed)

🌏 Real-World Validation

Tested on 10 SVAMITVA villages
Coverage includes:
Punjab
Chhattisgarh
🛠️ Tech Stack
🧠 Deep Learning: PyTorch
🧩 Segmentation: Segmentation Models PyTorch (SMP)
🤗 Transformers: Hugging Face Transformers
🗺️ Geospatial Processing: Rasterio · GeoPandas
🎨 Augmentation: Albumentations
🧭 Visualization & GIS: QGIS
👥 Team
👩‍💻 D. Sai Sudha Pavani
👩‍💻 K. Lasya Priya
👩‍💻 M. Bindu Madhavi
👨‍💻 B. Venkat Gopi Nayak
🎓 Dr. A. Ravi Raja

🏫 Institution:
Siddhartha Academy of Higher Education (Deemed to be University), Vijayawada

🧠 Mentorship & Challenge
🎯 Mentor: Geo-Intel Lab, IIT Tirupati Navavishkar I-Hub Foundation (IITTNiF)
🏆 Challenge: MoPR Geospatial Intelligence Hackathon 2025
🚀 Why This Matters

🌱 Enables accurate rural land mapping
🏡 Supports property ownership digitization (SVAMITVA)
📊 Reduces manual GIS effort drastically
🇮🇳 Scalable solution for nationwide deployment
