# MLSharp-TD-Bridge (2D to 3D Gaussian Splatting)

> **TouchDesigner 中的一键 2D 转 3D 高斯泼溅工具 | Portable AI Bridge** > **Author:** 多多GemosDodo

[中文版 (Chinese Version)](./README_zh-CN.md) | [English Version](./README.md)

<img width="1780" height="842" alt="image" src="https://github.com/user-attachments/assets/94273fd8-546f-41e1-b8c9-089944bb0463" />

## 项目简介 (Introduction)

**MLSharp-TD-Bridge** 是一个为 TouchDesigner 打造的便携式 AI 桥接工具。它基于 Apple 的 Sharp 模型架构，实现了**在 TouchDesigner 内部一键将 2D 图片转换为高质量 3D Gaussian Splatting（高斯泼溅）模型**。

传统的 AI 生成往往伴随着繁琐的 Python 环境配置、复杂的依赖安装（CUDA, PyTorch 等）以及命令行操作。本项目的目标是将这一过程彻底“自动化”与“黑盒化”。

**设计师无需编写任何代码，只需拖入图片，即可在几十秒内获得 3D 资产。**

## 💾 下载项目 (Download)

由于本项目内置了完整的便携式 Python 环境，文件体积较大，无法直接上传至 GitHub。**请务必通过下方的百度网盘链接下载完整的工程文件**。

**Due to GitHub file size limits (includes full portable Python env), please download the complete project via Baidu Netdisk:**

> **百度网盘 (Baidu Netdisk):** [点击下载 / Click to Download](https://pan.baidu.com/s/1CdKgvlUDEBoYldKr9qVYhw?pwd=czet)
> 
> **提取码 (Password):** `v3g3`

---

## 核心亮点 (Features)

* **零配置，即插即用 (Zero-Config)** 内置了完整的便携式 Python 环境（包含 PyTorch, CUDA, gsplat, sharp 等）。用户下载解压后，**无需安装 Anaconda**，直接运行 `.toe` 文件即可。

* **全自动工作流 (Fully Automated)** 点击一个按钮，脚本自动完成：`图像保存` -> `清理旧文件` -> `调用 AI 推理` -> `重命名文件` -> `刷新 3D 视图`。

* **TD 原生体验 (Native Integration)** * **Input**: 支持任意 TOP 图像源（Movie File In, Noise, etc.）。
    * **Output**: 生成结果自动回填至 Point File In，直接在 TD 视窗中预览。

* 🛠 **本地离线运行 (Offline Privacy)** 所有计算完全在本地 GPU 进行，无需联网，保护数据隐私。

## 系统要求 (Requirements)

* **操作系统**: Windows 10 / 11 (64-bit)
* **显卡**: NVIDIA 显卡 (建议显存 6GB 以上，支持 CUDA)
* **软件**: TouchDesigner 2022.x 或 2023.x 及以上版本

## 快速开始 (Getting Started)

1.  **下载项目 (Download)** 通过上方的**百度网盘链接**下载压缩包，并解压整个项目文件夹。  
    > **⚠️ 注意**：请确保解压后的路径中**不包含中文字符**（例如放 D 盘根目录），以免 Python 读取路径时报错。

2.  **启动工程 (Launch)** 双击运行文件夹内的 `MLSharp-TD-Bridge-by-GemosDodo.toe`。

3.  **一键生成 (Generate)** 选中 `Sharp_3D_Bridge` 组件，在属性面板点击 **`Generate`** 按钮。

4.  **查看结果 (View)** 等待约 30-60 秒（取决于显卡性能），生成的 3D 模型将自动加载到右侧的预览视窗中。

## 特别鸣谢 (Acknowledgements)

本项目还利用了由 **Yea Chen** 大佬开源的 **Touchdesigner 3D Gaussian Splatting Toolkits**，方便展示生成出来的高斯泼溅 3D 模型。

这也是本人制作的第一个开源项目，也是站在巨人的肩膀上了哈哈哈，本项目不做任何盈利，免费开源给各位，希望大家在 TD 的学习或者创作过程中使用愉快！！！！

* **ML_Sharp GitHub**：[https://github.com/apple/ml-sharp](https://github.com/apple/ml-sharp)
* **Touchdesigner 3D Gaussian Splatting Toolkits Github**：[https://github.com/yeataro/TD-Gaussian-Splatting](https://github.com/yeataro/TD-Gaussian-Splatting)
