# 🍓 StrawDet-YOLO

### A Real-Time and High-Precision Object Detector for Strawberry Disease Recognition

**StrawDet-YOLO** is a lightweight object detection model designed for fine-grained recognition of strawberry diseases, pests, and nutrient deficiencies under real-world agricultural conditions.

This repository provides the open resources associated with our paper **“StrawDet-YOLO: A Real-Time and High Precision Object Detection for Strawberry”**, published at the **2025 IEEE International Conference on Systems, Man, and Cybernetics (SMC)**, including the pretrained **PyTorch and ONNX model weights** and the **Strawberry-12 benchmark dataset**.

> **Paper:** [IEEE Xplore](https://ieeexplore.ieee.org/document/11343179/) · [DOI: 10.1109/SMC58881.2025.11343179](https://doi.org/10.1109/SMC58881.2025.11343179)  
> **Model Weights:** [PyTorch (.pt)](./weights/StrawDet-YOLO.pt) · [ONNX (.onnx)](./weights/StrawDet-YOLO.onnx)  
> **Dataset:** [Strawberry-12 on Hugging Face](https://huggingface.co/datasets/Ethan0300/Strawberry_12-dataset)

---

## 🔍 Overview

Accurate strawberry disease detection is challenging because symptoms can be subtle, visually similar, and strongly affected by complex field environments. **StrawDet-YOLO** is developed as a lightweight yet high-precision detector based on YOLOv8, targeting practical strawberry health monitoring and smart agricultural deployment.

The framework contains three key improvements:

- **BFSA — Bilinear Fused Synergic Attention:** refines spatial-channel attention fusion to improve sensitivity to subtle disease features.
- **R-SCConv — Residual Spatial and Channel Convolution:** enhances robust multi-scale feature reconstruction for complex visual patterns.
- **GWIoU — Gradient-Weighted IoU Loss:** dynamically emphasizes hard samples and improves bounding-box localization.

In the experiments reported in the paper, StrawDet-YOLO achieves a **7.7% precision improvement over YOLOv8n**, with superior mAP while maintaining **real-time inference at 0.4 ms per image**.

---

## 🚀 Model Weights

The pretrained **StrawDet-YOLO** model weights are publicly available in both **PyTorch (.pt)** and **ONNX (.onnx)** formats to support academic research, reproducibility, inference, and downstream deployment.

| Model | Format | Status | Download |
| --- | --- | --- | --- |
| **StrawDet-YOLO** | PyTorch (.pt) | ✅ Available | [**StrawDet-YOLO.pt**](./weights/StrawDet-YOLO.pt) |
| **StrawDet-YOLO** | ONNX (.onnx) | ✅ Available | [**StrawDet-YOLO.onnx**](./weights/StrawDet-YOLO.onnx) |

The released files are located at:

```text
weights/
├── StrawDet-YOLO.pt
└── StrawDet-YOLO.onnx
```

- **PyTorch checkpoint (.pt):** provided for researchers who prefer to work with the model in a PyTorch-based workflow.
- **ONNX model (.onnx):** provided for portable inference and deployment across different runtime environments.

> **Release scope:** This repository currently releases the pretrained model weights. The complete training source code and implementation files are not included in this release.

---

## 🍓 Strawberry-12 Dataset

**Strawberry-12** is the benchmark dataset constructed as part of the StrawDet-YOLO work. It contains strawberry diseases, pests, and nutrient deficiency symptoms collected under diverse real-world conditions.

| Item | Details |
| --- | --- |
| **Images** | 3,906 |
| **Annotations** | 16,107 bounding boxes |
| **Categories** | 12 |
| **Annotation Format** | YOLO (`.txt` per image) |
| **Collection Period** | Apr 2022 – Oct 2023 |
| **Environments** | Greenhouse and open-field |

Field data were collected across three growing seasons and cover four major strawberry varieties, providing diverse conditions for evaluating robust strawberry health detection.

📦 **Dataset download:** [Ethan0300/Strawberry_12-dataset on Hugging Face](https://huggingface.co/datasets/Ethan0300/Strawberry_12-dataset)

---

## 📁 Repository Structure

```text
Strawberry_12-dataset/
├── weights/
│   ├── README.md
│   ├── StrawDet-YOLO.pt
│   └── StrawDet-YOLO.onnx
├── LICENSE
└── README.md
```

---

## 📄 Paper

**StrawDet-YOLO: A Real-Time and High Precision Object Detection for Strawberry**  
Yue Hu, Xiankun Jiang, Jianfeng Guan  
*2025 IEEE International Conference on Systems, Man, and Cybernetics (SMC)*, pp. 6791–6797.

[IEEE Xplore](https://ieeexplore.ieee.org/document/11343179/) · [DOI](https://doi.org/10.1109/SMC58881.2025.11343179)

---

## 📝 Citation

If you find **StrawDet-YOLO**, its pretrained model, or the **Strawberry-12** dataset useful in your research, please cite our paper:

```bibtex
@INPROCEEDINGS{11343179,
  author={Hu, Yue and Jiang, Xiankun and Guan, Jianfeng},
  booktitle={2025 IEEE International Conference on Systems, Man, and Cybernetics (SMC)},
  title={StrawDet-YOLO: A Real-Time and High Precision Object Detection for Strawberry},
  year={2025},
  volume={},
  number={},
  pages={6791-6797},
  keywords={Location awareness;Smart agriculture;Accuracy;Spraying;Object detection;Nutrients;Real-time systems;Stability analysis;Monitoring;Diseases},
  doi={10.1109/SMC58881.2025.11343179}
}
```

---

## 📜 License

Please refer to the [LICENSE](./LICENSE) file for licensing information.
