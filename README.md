# Forest ROad STereo-camera Dataset (FROST)

This dataset contains synchronized RGB images, depth maps, and YOLO-format segmentation labels for forest road scene analysis.  
It is intended for research on road understanding, path detection, and segmentation tasks.

---

## 🌐 Dataset Download

The **Forest Road Segmentation Dataset** is hosted by **Graz University of Technology (TU Graz)** and can be downloaded from the official cloud storage:

**🔗 Download page:**  
👉 **[TU Graz – Forest Road Segmentation Dataset](https://cloud.tugraz.at/index.php/s/7ATWiRSXwtm9NRX)**

The website provides access to the full dataset, including RGB images, depth maps, and corresponding YOLO segmentation labels.

---

## 📂 Dataset Structure

dataset/ \
├── images/ # RGB images (JPEG/PNG) \
├── depths/ # Depth images aligned with the RGB images \
└── labels/ # YOLO segmentation labels (TXT files)


Each file in `images/`, `depths/`, and `labels/` shares the same base filename.  
Example:

images/000123.png \
depths/000123.png \
labels/000123.txt 


---

## 🧾 Label Format

Each label file follows the **YOLO COCO-style segmentation format**:

class_id x1 y1 x2 y2 ... xn yn


- Each line represents one polygon corresponding to a class instance.  
- Coordinates are **normalized** (values between 0 and 1).  
- Multiple polygons may exist per file.

---

## 🏷️ Class Definitions

| ID | Class Name     |
|----|----------------|
| 0  | Road           |
| 1  | Road Boundary  |

---

## 📜 License

**License:** CC BY-NC-SA 
You are free to share and adapt the dataset with appropriate credit.  
Please cite this dataset if used in research or publications.
