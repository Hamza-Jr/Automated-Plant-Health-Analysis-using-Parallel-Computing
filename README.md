# **Automated Plant Health Analysis using Parallel Computing** 🌿🚀  

## **📌 Project Overview**  
This project focuses on **automated plant detection, counting, and health assessment** using **NDVI (Normalized Difference Vegetation Index) and NDWI (Normalized Difference Water Index)**. By leveraging **parallel computing techniques (CUDA, OpenCL, OpenMP)**, the system significantly speeds up image processing for large datasets.  

---

## **📂 Table of Contents**  
- [📖 Introduction](#-introduction)  
- [📂 Dataset](#-dataset)  
- [⚙️ Dependencies](#-dependencies)  
- [🛠️ Processing Pipeline](#-processing-pipeline)  
- [📊 Visualization Results](#-visualization-results)  
- [📊 Performance Comparison](#-performance-comparison)  

---

## ** Introduction**  
This project aims to **automate plant health analysis** by processing **RGB and NIR (Near Infrared) images** to compute vegetation indices such as **NDVI** and **NDWI**. The key features include:  

✅ **Automated Plant Detection & Counting** – No manual field inspection required.  
✅ **Parallelized Processing** – CUDA, OpenCL, and OpenMP accelerate image analysis.  
✅ **Precision Health Monitoring** – NDVI/NDWI values indicate plant health.  
✅ **Interactive Visualization** – Color-coded field representation for insights.  

---

## ** Dataset**  
The dataset consists of **306 RGB and NIR images** of an agricultural field with a resolution of **1296×966 pixels**.  
Each image is processed to extract plant-specific health data.  
📷 **Example Input RGB Image**  
![RGB Image](./images/rgb_example.jpg)  

📷 **Example Input NIR Image**  
![NIR Image](./images/nir_example.jpg)  

---

## ** Dependencies**  
Before running the project, install the required dependencies:  

bash
pip install numpy pandas opencv-python matplotlib


---

## **Processing Pipeline**  
**1-Load Images:**

Reads RGB and NIR images.
Converts images into a format suitable for processing.

**2-Compute NDVI & NDWI**

Extracts vegetation indices from image data.
Identifies stress levels in plants based on reflectance properties.

**3-Instance Segmentation**

Detects and segments individual plants using contour detection.
Filters out noise and non-plant objects.

**4-Annotation & Visualization**

Highlights plants with bounding boxes.
Displays NDVI and NDWI values for each detected plant.

**5-Performance Optimization**

Utilizes parallel computing (CUDA, OpenCL, OpenMP) to accelerate processing.
 



---

## ** Visualization Results**  
The following images illustrate different stages of processing:

📷 Input RGB and NIR Images
![RGB Image](./images/rgb_example.jpg)  
![RGB Image](./images/rgb_example.jpg)  

Raw RGB and Near-Infrared (NIR) images used for analysis.
📷 NDVI and NDWI Computation
![RGB Image](./images/rgb_example.jpg)  

False-color maps representing vegetation health and water content.
📷 Segmented & Annotated Images
![RGB Image](./images/rgb_example.jpg)  

Each detected plant is highlighted with bounding boxes and labeled with health indices.
📷 Performance Benchmark Graphs
![RGB Image](./images/rgb_example.jpg)  






---

## ** Performance Comparison**  

Visual comparisons of processing speed improvements across different parallelization methods.
![RGB Image](./images/rgb_example.jpg)  








