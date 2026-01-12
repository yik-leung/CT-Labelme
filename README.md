# CT-LabelMe 🩻

**An extremely simple and doctor-friendly CT annotation tool**  
Designed for fast correction of AI-generated segmentations

[![Python](https://img.shields.io/badge/python-3.11+-blue)](https://www.python.org/)


## 🎯 Motivation

From my own experience collaborating closely with many radiologists and clinicians over the years, I observed that about 95 % of the doctors I worked with had no idea how to use a GPU to run AI, and had no interest in investing time to learn medical image annotation software such as ITK-SNAP or 3D Slicer, let alone exploring and installing advanced interactive AI plugins like nnInteractive inside those tools.

Besides, in my actual projects, the typical workflow is AI generating coarse initial labels first, with clinicians mainly performing quick corrections afterward. Inspired by this pattern, I decided to create a very lightweight, easy-to-use annotation tool, keeping things as simple and frictionless as possible.

## ✨ Features

- Supports common medical formats: NRRD • DICOM • NIfTI (.nii.gz)
- Automatic window/level adjustment optimized for CT
- Automatic slice interpolation
- Uses 3D bounding box coordinates to greatly reduce voxel computation load, enabling efficient handling of large CT stacks with thousands of slices.
- ...
- ...
- More features and detailed instructions: click the **Help** button in the menu

Future plans: Support interactive polygon annotation (vertices saved separately in JSON file)

## 🚀 Installation

### Option 1: Windows users (zero installation)

Just download the latest `CT-LabelMe.exe` and double-click the file.

### Option 2: pip (Mac / Ubuntu / advanced Windows users)

```bash
git clone https://github.com/yourusername/CT-LabelMe.git
cd CT-LabelMe
pip install -r requirements.txt
python main.py
```

## ⌨️ Quick Start & Hotkeys

<p align="center">
  <img src="https://github.com/user-attachments/assets/fd47db48-106e-4081-a7a3-1d9437900e9f" alt="CT-LabelMe Demo" width="800"/>
</p>

About the hotkeys, please click the **Help** button in the menu

## 🙏 Acknowledgments

- Core annotation logic inspired by **[labelme](https://github.com/wkentaro/labelme)**.
- Core voxel handling from **[Med-labelme](https://github.com/MeteorsHub/MedLabelMe)**.

## 📄 Citation

If you find CT-LabelMe useful in your work, please consider citing:

```bibtex
@misc{CTLabelMe,
  author  = {Yiliang Chen},
  year = {2025},
  journal = {Github repository},
  title = {A Simple Lightweight CT Annotation Tool},
  howpublished = {\url{https://github.com/yik-leung/CT-Labelme}}
}
