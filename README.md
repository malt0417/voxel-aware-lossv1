# voxel-aware-lossv1
# Voxel-Aware Loss (3D Medical Imaging)

> Physically consistent, anisotropy-aware losses for 3D medical imaging.  
> **Weighted L1** with voxel-volume and spacing-aware gradient consistency.

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)]()
[![PyTorch](https://img.shields.io/badge/PyTorch-1.12%2B-red)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)]()

## ✨ Features
- **Voxel-volume aware L1**: treats the discrete loss as a Riemann sum over anisotropic voxels.
- **Spacing-weighted gradient consistency**: balances x/y/z differences via `(1/sx, 1/sy, 1/sz)`.
- **Batch-wise spacing**: support for per-sample spacings of shape `[B, 3]`.
- **Plug-and-play**: drop-in PyTorch `nn.Module`.

## 📦 Install
```bash
pip install -U pip
pip install -e .
