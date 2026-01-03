# Sharp-TD-Bridge (2D to 3D Gaussian Splatting)

> **One-click 2D to 3D Gaussian Splatting Tool for TouchDesigner | Portable AI Bridge** > **Author:** GemosDodo

[中文版 (Chinese Version)](./README_zh-CN.md) | [English Version](./README.md)

<img width="1780" height="842" alt="image" src="https://github.com/user-attachments/assets/94273fd8-546f-41e1-b8c9-089944bb0463" />

## Introduction

**Sharp-TD-Bridge** is a portable AI bridge tool built specifically for TouchDesigner. Based on Apple's **Sharp** model architecture, it achieves **one-click conversion of 2D images into high-quality 3D Gaussian Splatting models directly within TouchDesigner**.

Traditional AI generation often involves tedious Python environment configuration, complex dependency installations (CUDA, PyTorch, etc.), and command-line operations. The goal of this project is to completely "automate" and "black-box" this process.

**Designers do not need to write a single line of code. Simply drag in an image, and obtain 3D assets within seconds.**

## Features

* **Zero-Config & Plug-and-Play** Includes a complete portable Python environment (containing PyTorch, CUDA, gsplat, sharp, etc.). After downloading and unzipping, there is **no need to install Anaconda**. Just run the `.toe` file directly.

* **Fully Automated Workflow** With a single button click, the script automatically handles: `Save Image` -> `Clean Old Files` -> `AI Inference` -> `Rename Files` -> `Refresh 3D View`.

* **Native TouchDesigner Integration** * **Input**: Supports any TOP image source (Movie File In, Noise, etc.).
    * **Output**: Generated results are automatically loaded back into a Point File In for immediate preview in the TD viewport.

* 🛠 **Offline Privacy** All calculations are performed locally on your GPU. No internet connection is required, ensuring data privacy.

## Requirements

* **OS**: Windows 10 / 11 (64-bit)
* **GPU**: NVIDIA GPU (Recommended: 6GB+ VRAM, CUDA support required)
* **Software**: TouchDesigner 2022.x or 2023.x and above

## Getting Started

1.  **Download the Project** Download and unzip the entire project folder.  
    > **Note**: Please ensure the unzipped path **does not contain non-English characters** (e.g., placing it at the root of the D drive is recommended) to avoid Python path errors.

2.  **Launch the Project** Double-click to run `MLSharp-TD-Bridge-by-GemosDodo.toe`.

3.  **One-Click Generation** Select the `Sharp_3D_Bridge` component. In the custom parameters panel, click the **`Generate`** button.

4.  **View Results** Wait for approximately 30-60 seconds (depending on GPU performance). The generated 3D model will automatically load into the preview window on the right.

## Acknowledgements

This project utilizes the **TouchDesigner 3D Gaussian Splatting Toolkits** open-sourced by **Yea Chen** to visualize the generated Gaussian Splatting 3D models.

This is my first open-source project, standing on the shoulders of giants. This project is non-profit and free for everyone. I hope you enjoy using it in your TouchDesigner learning or creative process!

* **ML_Sharp GitHub**: [https://github.com/apple/ml-sharp](https://github.com/apple/ml-sharp)
* **TouchDesigner 3D Gaussian Splatting Toolkits**: [https://github.com/yeataro/TD-Gaussian-Splatting](https://github.com/yeataro/TD-Gaussian-Splatting)
