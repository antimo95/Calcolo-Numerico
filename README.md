# 📊 MATLAB Numerical Methods App & NURBS Theory

![MATLAB](https://img.shields.io/badge/MATLAB-R2021a-orange) ![App Designer](https://img.shields.io/badge/App-Designer-blue) ![Numerical%20Analysis](https://img.shields.io/badge/Numerical-Analysis-green) ![CAD](https://img.shields.io/badge/CAD/NURBS-gray)

---

## 📌 Project Overview
This project collects **three interactive numerical analysis applications in MATLAB**, developed with **App Designer**, together with a **theoretical study on NURBS** (Non-Uniform Rational B-Splines).  

The main goals are:
- Implement and compare **numerical interpolation techniques**  
- Analyze real-world datasets with **smoothing and regression**  
- Apply interpolation to **image contour tracking and resizing**  
- Provide a **theoretical foundation on NURBS**, widely used in **3D graphics and CAD**  

---

## 📂 Project Structure
- **menu.mlapp** → main interface (navigation panel)  
- **Interpolazione.mlapp**
  - Polynomial interpolation  
  - Piecewise linear interpolation  
  - Cubic splines (not-a-knot, natural)  
  - Maximum error computation  
- **crescitademografica.mlapp**
  - Italian population analysis (1946–2020)  
  - 2021 prediction with spline  
  - Least squares regression (line & parabola)  
  - Euro/Dollar exchange rate analysis (with/without noise)  
- **tracking_miglioria.mlapp**
  - Image contour tracing with spline interpolation  
  - Image resizing with **nearest**, **bilinear**, **bicubic** interpolation  
  - Visual quality comparison  
- **NURBS Section**
  - Theory and mathematical definition  
  - Relation with Bézier and B-Splines  
  - Properties and shape manipulation  
  - Applications in **Rhino 7 CAD**  

---

## 🛠 Tools & Technologies Used
- **MATLAB R2021a**  
- **App Designer** for GUI development  
- MATLAB Functions:  
  - `polyfit`, `polyval` → polynomial fitting  
  - `interp1` → linear interpolation  
  - `spline`, `csape` → cubic splines  
  - `dlmread` → external data import  
  - `imread`, `imshow`, `imresize` → image processing  
  - `ginput` → manual node selection on images  
- **Rhino 7** for CAD-based NURBS modeling  

---

## 📊 Numerical Analysis & Implementation
### 🔍 Interpolation
- Tested on known functions (e.g., `sin(x)`)  
- Compared polynomial, piecewise linear, and cubic spline interpolation  
- Evaluated maximum error (∞-norm)  

👉 **Result**: natural cubic splines provide the most accurate and stable interpolation.  

### 📈 Smoothing & Prediction
- Italian population dataset (1946–2020)  
- 2021 prediction with spline interpolation  
- Least squares fitting (line & parabola)  
- Euro/Dollar exchange rate analysis with noisy and corrected data  

👉 **Result**: splines are effective for local trends, least squares for global trends.  

### 🖼 Image Tracking & Resizing
- Image contour tracing using manually selected nodes and spline interpolation  
- Image resizing using:  
  - Nearest neighbor (fast but poor quality)  
  - Bilinear (good compromise)  
  - Bicubic (best visual quality)  

👉 **Result**: bicubic interpolation yields the best quality, though computationally heavier.  

---

## 📐 NURBS – Theoretical Insights
**NURBS (Non-Uniform Rational B-Splines)** are a generalization of Bézier and B-Spline curves, widely used in **3D graphics and CAD** for curve and surface modeling.  

### 🔹 Applications
- Complex surface modeling in **CAD/CAM**  
- 3D graphics & animation  
- **Rhinoceros 7** → all geometric entities are represented as NURBS  

---

## 📈 Results & Conclusion
- **Natural cubic splines** = best method for interpolation  
- **Spline smoothing** effective for noisy data & local prediction  
- **Bicubic interpolation** = best image resizing technique  
- **NURBS** = powerful tool bridging **numerical analysis and geometric modeling**  

📌 **Conclusion**: This project highlights how **numerical methods** can be applied to real-world problems (data analysis, images) while also connecting to advanced theoretical tools (NURBS), bridging the gap between **numerical computation and CAD modeling**.  

---

## 👨‍💻 Authors
- Francesco Erminio Di Fruscio (M631004)  
- Antimo Barbato (M631079)  
