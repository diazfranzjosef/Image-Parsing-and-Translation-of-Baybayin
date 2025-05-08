ᜋᜊᜓᜑᜌ᜔!
This project focuses on building, training, and evaluating a YOLOv8-based deep learning system for the detection and recognition of Baybayin script characters at the document level. The project involves custom dataset creation, augmentation, model training, evaluation, and post-processing to reconstruct the document’s text flow.

Methods Overview

Dataset Preparation
  Custom Baybayin document images were manually written, annotated, and prepared.
  Augmentation techniques (flipping, blurring, affine transforms, etc.) were applied to increase data variability.
  Dataset was formatted for YOLOv8 training.

Model Training
  YOLOv8 was trained using the prepared dataset.
  Training used hyperparameter tuning (epochs=100, imgsz=64, batch=16, lr=0.0010) for optimal results.
  Pretrained weights were used with minimal architecture changes.

Model Evaluation
  Performance was validated using precision, recall, mAP50, and mAP50–95 metrics.
  Multiple runs were conducted, showing consistent improvement as the dataset and augmentation methods improved.

Inference and Post-processing
  Predictions were sorted left-to-right, top-to-bottom to reconstruct document character sequences.
  Outputs were visualized and analyzed to assess real-world applicability.

How to Run:

Clone the repository:
git clone <repo-url>
cd <repo-folder>

Install required packages:
pip install ultralytics opencv-python albumentations matplotlib

Run the training notebook and inference.

For any questions, reach out to diazfranzjosef@gmail.com

ᜐᜎᜋᜆ᜔
