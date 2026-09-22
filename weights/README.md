# 🚀 StrawDet-YOLO Model Weights

This directory contains the released pretrained model weights for **StrawDet-YOLO**, introduced in:

> **StrawDet-YOLO: A Real-Time and High Precision Object Detection for Strawberry**  
> Yue Hu, Xiankun Jiang, Jianfeng Guan  
> 2025 IEEE International Conference on Systems, Man, and Cybernetics (SMC)

## Available Checkpoints

| Model | Format | File |
| --- | --- | --- |
| **StrawDet-YOLO** | PyTorch (.pt) | [`StrawDet-YOLO.pt`](./StrawDet-YOLO.pt) |
| **StrawDet-YOLO** | ONNX (.onnx) | [`StrawDet-YOLO.onnx`](./StrawDet-YOLO.onnx) |

### PyTorch Checkpoint

The `.pt` checkpoint is provided for researchers who prefer to use the pretrained StrawDet-YOLO model in a PyTorch-based workflow.

### ONNX Model

The `.onnx` model is provided for portable inference and deployment across different runtime environments.

> **Release scope:** This repository currently releases the pretrained model weights only. The complete training source code and implementation files are not included in this release.

## Paper

- [IEEE Xplore](https://ieeexplore.ieee.org/document/11343179/)
- [DOI: 10.1109/SMC58881.2025.11343179](https://doi.org/10.1109/SMC58881.2025.11343179)

## Citation

If you use the released model weights in your research, please cite the original paper:

```bibtex
@INPROCEEDINGS{11343179,
  author={Hu, Yue and Jiang, Xiankun and Guan, Jianfeng},
  booktitle={2025 IEEE International Conference on Systems, Man, and Cybernetics (SMC)},
  title={StrawDet-YOLO: A Real-Time and High Precision Object Detection for Strawberry},
  year={2025},
  pages={6791-6797},
  doi={10.1109/SMC58881.2025.11343179}
}
```
