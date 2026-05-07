# 🧠 3D Brain Segmentation from CT Scan

## 📌 Overview
This project demonstrates the segmentation and 3D reconstruction of brain tissue from CT imaging data using 3D Slicer.

The goal was to isolate brain structures from surrounding anatomy (e.g., skull and soft tissue) and generate a clean 3D surface model suitable for visualization and further analysis.

---

## 🛠️ Methods

The segmentation pipeline included:

- Intensity-based thresholding to isolate relevant tissue ranges  
- Manual refinement using painting and scissor tools  
- Region-based cleanup to remove non-brain structures  
- Surface smoothing to reduce segmentation noise  
- 3D reconstruction using closed surface generation  

All processing was performed in **3D Slicer**.

---

## 📸 Results

### Front
![Front](front.png)

### Back
![Back](back.png)

### Left
![Left](left.png)

### Right
![Right](right.png)

### Inferior View
![Under](under.png)

---

## 📦 Files

- **brain_segmentation.stl** → Final 3D surface model of the segmented brain  
- **segmentation.seg.nrrd** → Segmentation data file (for reproducibility in 3D Slicer)

---

## 📚 Data Source

CT data derived from publicly available datasets via:

- The Cancer Imaging Archive (TCIA)  
- Google DeepMind medical imaging dataset  

---

## 🎯 Applications

This workflow demonstrates skills relevant to:

- Medical image processing  
- Biomedical engineering  
- Computational anatomy  
- 3D reconstruction from volumetric data  

---
## 📊 Quantitative Analysis

Brain segmentation was analyzed using 3D Slicer’s Segment Statistics module.

### Key Metrics
- Volume: **1,111,200 mm³** (1111.2 cm³)
- Voxel Count: **462,809**
- Mean Intensity: **30.83**

These values were extracted directly from the segmented region to quantify anatomical structure from CT imaging.

📄 Full dataset available here: [segment_statistics.tsv](segment_statistics.tsv)

---
## 📄 License

This project is released under the MIT License.
