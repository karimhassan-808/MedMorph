# MedMorph# 🧠 MedMorph

> *Morph your medical scans into clarity.*  

**MedMorph Editor** is a comprehensive application designed for **processing and analyzing medical image data**, especially in the DICOM format. With a suite of advanced tools for **editing, visualizing, and enhancing** images, it’s perfect for researchers, students, and professionals in the medical imaging field.

Built with 💡 **PyQt5**, 🔧 **OpenCV**, and 🩺 **pydicom**, it brings a smooth GUI experience fused with hardcore image processing capabilities.

---

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
    ```bash
    pip install -r requirements.txt
    ```

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

# Photo
![Image](https://github.com/user-attachments/assets/f9074268-bcd3-4b80-968b-74779208a2be)
![Image](https://github.com/user-attachments/assets/598be92a-aaba-44f2-9be6-ac1f54463331)
![Image](https://github.com/user-attachments/assets/98e3d1d9-3ee5-440a-bebd-aaf3a0318281)
![Image](https://github.com/user-attachments/assets/ac144c23-a43b-4b4e-b2df-174317852af5)
![Image](https://github.com/user-attachments/assets/97042fde-1a02-45d1-9b21-f7403167a035)
![Image](https://github.com/user-attachments/assets/844a5bdf-d14c-4fea-80e2-32eec75b85ee)
![Image](https://github.com/user-attachments/assets/f1632ce5-2bcd-4326-8fd4-b81f6c67b6d0)

# Video
https://github.com/user-attachments/assets/d20863aa-3f4d-4439-a057-003a3fc4bc4e
## License
This project is licensed under the [MIT License](LICENSE).