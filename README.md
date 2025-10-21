# Image-Forgery-Detection
A deep learning model for detecting image forgery using Error Level Analysis and Convolutional Neural Networks (CNN). Implements feature enhancement using CBAM attention for improved accuracy.

Our model leverages Error Level Analysis (ELA) for preprocessing and a Convolutional Neural Network (CNN) integrated with Convolutional Block Attention Module (CBAM) for enhanced feature extraction and classification accuracy.

The dataset used is CASIA 2.0 having 12614 images out of which 7491 are real and 5123 are tampered images.

**Overview**

The project pipeline involves three major components:

Error Level Analysis (ELA) — A preprocessing technique that highlights compression artifacts in an image, helping to reveal manipulated regions.

CNN Model — Learns discriminative features from ELA-transformed images to classify them as real or forged.

CBAM Attention Module — Improves model focus by adaptively refining spatial and channel-wise feature maps.

**Key Features**

Preprocessing using Error Level Analysis (ELA)

Deep learning-based CNN classifier

Integration of CBAM (Channel and Spatial Attention) for performance enhancement

Detects both splicing and copy-move forgeries

Supports custom datasets and image-level classification

**Architecture**
Input Image → ELA Preprocessing → CNN Layers → CBAM Attention → Fully Connected Layers → Output (Real / Forged)
The CBAM module enables the network to automatically learn where to look in the image, improving detection of subtle tampering cues.
