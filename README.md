🚦 Traffic Sign Classification System
This repository contains a deep learning project that builds and compares multiple computer vision models to classify German traffic signs using the GTSRB dataset.

📁 Dataset Source
Name: GTSRB - German Traffic Sign Recognition Benchmark


Description: 39,000+ labeled images across 43 traffic sign classes.

Image Size: Resized to (96x96x3) for compatibility with MobileNetV2.

🧠 Models Compared
Model	 Train Accuracy	  Val Accuracy	   
CNN (no augmentation)	98.8%	99.63%	  

CNN + augmentation	96.1%	99.62%	  

MobileNetV2 (fine-tuned)	92.3%	59.9%

🔧 Custom CNN: Built from scratch using Conv2D, MaxPooling, Dense, and Dropout.

🔄 Transfer Learning: Fine-tuned MobileNetV2 with last 30 layers trainable.

🔄 Data Augmentation Techniques
To improve generalization, the following augmentations were applied:

rotation_range=15

width_shift_range=0.1

height_shift_range=0.1

zoom_range=0.1

shear_range=0.1

📊 Evaluation & Results
Best Model: CNN with data augmentation

Limitations: MobileNetV2 underperformed due to domain mismatch

Visuals: Confusion matrices and training plots are available in the results/ folder.

🧰 Features
Image resizing and normalization

One-hot encoding for labels

Training/validation split

Data augmentation

Model evaluation: accuracy & confusion matrix

Model saving (.h5 format)

📄 License

This project is intended for educational and research purposes as part of the Elevvo Pathways ML Internship.

👨‍💻 About
Traffic sign classification using deep learning.
Includes custom CNN, MobileNetV2, data augmentation, transfer learning, and visual evaluation metrics.

