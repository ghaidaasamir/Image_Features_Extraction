# Feature Matching with ORB (Oriented FAST and Rotated BRIEF) 

Feature detection and matching between images using **ORB**, a fast and efficient algorithm for feature extraction and matching.

---


### **1. Feature Detection using ORB**
- The **ORB detector** finds key points.  
- Each key point is assigned a **descriptor** that represents its features.  
- The detected key points are **drawn on the image** for visualization.

### **2. Feature Matching**
- Two images are loaded and converted to **grayscale** (better for feature detection).  
- The ORB detector extracts **key points and descriptors** for both images.  
- A **Brute-Force Matcher (BFMatcher)** is used to compare descriptors and find **similar features** in both images.  
- The best matches are drawn to **visualize** the similarity between images.

---

## **Files**  
- **`book1.png` & `book3.png`**  Sample images for feature matching.  
- **`features_extraction.ipynb`**  Runs ORB detection and matching.

---

## **Setup & Installation**  
1. **Install dependencies:**  
   ```bash
   pip install opencv-python matplotlib numpy
   ```

2. **Run:**  
   ```bash
   features_extraction.ipynb
   ```

---

## **Example**  
### **Feature Detection**
- ORB detects **key points** in `book1.png`.  
- The detected points are **drawn on the image**.  

### **Feature Matching**
- ORB compares `book1.png` and `book3.png`.  
- **Matching points** are displayed with lines showing correspondences.  
