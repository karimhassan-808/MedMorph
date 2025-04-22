# 🧠 MedMorph

> *Morph your medical scans into clarity.*  

**MedMorph Editor** is a comprehensive application designed for **processing and analyzing medical image data**, especially in the DICOM format. With a suite of advanced tools for **editing, visualizing, and enhancing** images, it’s perfect for researchers, students, and professionals in the medical imaging field.

Built with 💡 **PyQt5**, 🔧 **OpenCV**, and 🩺 **pydicom**, it brings a smooth GUI experience fused with hardcore image processing capabilities.

---
## Project Structure 📂
```
  MedMorphProject/
    ├── src/              # Source code directory
    │   └── MedMorph/     # Main application code
    ├── Data for testing/             # Sample/test DICOM data
    ├── README.md         # Project documentation (this file)
    ├── requirements.txt  # Python dependencies
    └── .gitignore        # Git ignore rules
```
    
## 🚀 Features

### 🖼️ Image Processing & Enhancement
- Add noise: **Gaussian**, **Salt & Pepper**, **Pink noise**
- Apply filters: **Gaussian**, **Median**, **Pink**, **High-pass**, **Low-pass**
- Adjust **contrast** and **brightness**
- Advanced enhancements:
  - 📊 Histogram Equalization
  - ⚡ CLAHE (Contrast Limited Adaptive Histogram Equalization)
  - 🔬 Morphological Enhancements

### 📈 SNR & CNR Analysis
- Interactive ROI-based selection
- Real-time updates for:
  - **Signal-to-Noise Ratio (SNR)**
  - **Contrast-to-Noise Ratio (CNR)**

### 🔍 Zoom & Resolution Tools
- Dynamic zoom (in/out) with interpolation:
  - Nearest-Neighbor
  - Bilinear
  - Cubic
- Resolution scaling for fast rendering

### 📉 Histogram Viewer
- Displays **detailed pixel intensity histograms** with:
  - Mean
  - Median
  - Standard Deviation

### 🛡️ Robust Error Handling
- Clean feedback for unsupported files
- Handles large datasets like a champ

---

## 🧩 File Content

### 🧱 Classes
- **`AnalysisLabel`** – Handles image interaction and zoom logic
- **`MainWindow`** – Main GUI & logic orchestrator

### 🧠 Key Functions

#### 🔄 File Loading
- `import_dicom` – Load & normalize DICOM files
- `normalize_image` – Converts pixel values to 8-bit

#### 🎛️ Image Editing
- `apply_contrast` – Contrast control
- `apply_brightness` – Brightness tuning
- `apply_resolution` – Dynamic resolution adjustment

#### 🧪 Enhancement
- `apply_histogram_equalization`
- `apply_clahe`
- `apply_morphological_enhancement`

#### 📊 Analysis
- `perform_snr_analysis` – SNR/CNR from selected ROIs
- `delete_analysis_boxes` – Reset boxes & results

#### 🔎 Zoom & Navigation
- `zoom_in / zoom_out` – Zoom functions
- `select_viewport` – Switch image views

---

## 🛠️ Usage

### 1. 📦 Install Dependencies
    pip install -r requirements.txt
    

### 2. Fire It Up 🚀
    run python MedMorph.py

### 3.  Load a DICOM Image 📂
    Click that "Import DICOM" button and choose your, dcm file

### 4. Edit & Enhance 🎨
    Get creative with the toolbar:
    - Add noise for a gritty look 🎲
    - Apply filters to refresh the vibe 🔄
    - Adjust contrast, brightness, or resolution to perfection 🌟
    - Want to go next-level? Try CLAHE or Histogram Equalization for some serious enhancement 🔧

### 5. Analyze Like a Scientist 🔬
    Activate the SNR/CNR analysis, pick your regions of interest, and watch the metrics pop up as the app dynamically updates 📊

### 6. Zoom In for the Details 🔍
    Zoom in to focus on the fine details 🧐, Adjust interpolation for that ultra-smooth viewing experience ✨

### 7.  Dive Into the Histogram 📈
    Double-click on an image to open the histogram. Get the lowdown on the stats and see your image in a whole new light 💡

### 8. Wrapping Up 🏁
    Done? Close the window or terminate the app from the command line and call it a day 🙌

# Illustrations 🎨
## Gussian noise, denoise
  ![Image](https://github.com/user-attachments/assets/a978d7d7-6728-423d-a9ca-fea02c114a5f)
## High, Low pass Filters
  ![Image](https://github.com/user-attachments/assets/caabbacb-d54a-43d6-addd-f18cd84d7824)
## Histogram Equalization, CLAHE
  ![Image](https://github.com/user-attachments/assets/6d81a57b-dc17-4012-bd16-f8970c95fe2d)
## Pink noise, denoise
  ![Image](https://github.com/user-attachments/assets/95f33cdb-ff9b-4c9e-9e8e-57d9a05b5d62)
## Salt and Pepper noise, denoise
  ![Image](https://github.com/user-attachments/assets/18c45333-6848-4b1f-9d96-86d16153cfc9)
## SNR and CNR
  ![Image](https://github.com/user-attachments/assets/0ace14af-ecfa-4bb9-95fb-a3cb169f94b1)
## Zooming Techniques
  ![Image](https://github.com/user-attachments/assets/d8307497-6373-41df-a875-ac138ec4ce47)
# Video
[https://github.com/user-attachments/assets/d20863aa-3f4d-4439-a057-003a3fc4bc4e](https://github.com/user-attachments/assets/4f225e22-0790-436c-a4e3-5cd9868b95a8)

# Project Team 🧑‍🤝‍🧑

# Contributors
1. [Kareem Taha](https://github.com/Kareem-Taha-05)
2. [Omar Gamal](https://github.com/OmarGamalH)
3. [Karim Hassan](https://github.com/karimhassan-808)
4. [Omar Amein](https://github.com/OmarAmein)

## License
This project is licensed under the [MIT License](LICENSE).
