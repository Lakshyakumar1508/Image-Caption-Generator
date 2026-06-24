# 🖼️ Image Caption Generator using ResNet50 + Transformer

An AI-powered Image Captioning system that automatically generates natural language descriptions for images using **ResNet50** for visual feature extraction and a **Transformer Decoder** for caption generation.

---

## 🚀 Project Overview

This project combines Computer Vision and Natural Language Processing to generate meaningful captions for images.

### Architecture

```text
Input Image
      │
      ▼
 ResNet50 Encoder
 (2048 Features)
      │
      ▼
 Linear Projection
 (2048 → 512)
      │
      ▼
 Transformer Decoder
 (3 Layers, 8 Heads)
      │
      ▼
 Generated Caption
```

---

## 📂 Dataset

Dataset Used: **Flickr30k**

- ~31,000 Images
- ~158,000 Captions
- 5 Human-Annotated Captions per Image

---

## 🛠️ Tech Stack

- Python
- PyTorch
- Torchvision
- Transformers
- NumPy
- Pandas
- Matplotlib
- PIL
- tqdm

---

## 🔥 Model Details

### Encoder

- ResNet50 Pretrained on ImageNet
- Feature Vector Size: 2048

### Decoder

- Transformer Decoder
- Embedding Dimension: 512
- Number of Decoder Layers: 3
- Multi-Head Attention: 8 Heads
- Dropout: 0.1

### Training Configuration

| Parameter | Value |
|------------|---------|
| Batch Size | 64 |
| Learning Rate | 1e-4 |
| Optimizer | Adam |
| Loss Function | Cross Entropy Loss |
| Epochs | 40 |
| Gradient Clipping | 1.0 |

---

## 📊 Results

### Evaluation Metrics

| Metric | Score |
|----------|----------|
| BLEU-1 | **0.7706** |
| BLEU-4 | **0.4678** |
| CIDEr | **1.2838** |

### Performance Summary

✅ Strong caption generation quality

✅ High semantic similarity with ground-truth captions

✅ CIDEr score above 1.2 indicating excellent caption relevance

---

## 📸 Sample Output

### Input Image

Image: 106514190.jpg

Predicted Caption:
skier is overlooking the beautiful white snow covered landscape

Ground Truth Captions:
1. skier is overlooking the beautiful white snow covered landscape
2. hiker standing high on bluff overlooking the mountains below
3. person on ski looks from hill over snow covered landscape
4. skier is overlooking snowcovered mountain
5. skier pauses on mountaintop

====================================================================================================
Image: 2541483099.jpg

Predicted Caption:
workers in safety vests and hard hats work on tunnel

Ground Truth Captions:
1. men working wearing orange safety vests and hard hats in hallway
2. construction workers are working on the side panels of tunnel
3. construction workers laying wall tile in hallway
4. construction workers are working in tunnel
5. workers place tiles on walls


## 📈 Future Improvements

- Beam Search Decoding
- Attention Visualization
- Fine-Tuning ResNet50
- Vision Transformer (ViT) Encoder
- BLIP-Based Captioning
- Web Application Deployment

---

## 🎯 Key Achievements

- Built a complete Image Captioning Pipeline
- Implemented Transformer-based Caption Generation
- Achieved:
  - BLEU-1: **0.7706**
  - BLEU-4: **0.4678**
  - CIDEr: **1.2838**
- Trained on Flickr30k Dataset
- Generated human-like image descriptions

---

## 👨‍💻 Author

**Lakshya Kumar**

B.Tech CSE (AI & ML)  
Haridwar University

### Connect With Me

- LinkedIn: www.linkedin.com/in/lakshya-kumar-srivastava
- GitHub: https://github.com/Lakshyakumar150

---

## ⭐ If you found this project useful, give it a star!
