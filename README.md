# 2D-Shape-Prediction

📌 **Status:** This is a paper in progress. Below is a rough overview of what has been done so far.

This project explores forecasting the evolution of a 2D shape over time using radial sampling and time-series prediction techniques.

---

### Workflow Overview

✅ **Step 1 – Simulate Shape Evolution:**  
I manually created circular layers, each expanding slightly each year to simulate shape evolution over time.  
<img width="1200" height="729" alt="1  CIrcular layers" src="https://github.com/user-attachments/assets/5e00029c-4d5a-4a9a-9660-e702768e09e9" />

✅ **Step 2 – Extract Centroid and Generate Radial Lines:**  
Calculated the centroid of the first-year shape and created radial lines in 1-degree increments to cover the full circular boundary. 
<img width="1179" height="724" alt="2  Radial Line" src="https://github.com/user-attachments/assets/3a994d32-afe9-4445-b1a8-5e28ccd5fbb9" />

✅ **Step 3 – Intersect Shapes with Radial Lines:**  
Performed an intersection of each shape with the radial lines to extract geometry at each angle.  <img width="1162" height="699" alt="3  intersection lines" src="https://github.com/user-attachments/assets/9c9c040e-4e25-4e71-a7d8-5ff84fd1ebfc" />

✅ **Step 4 – Predict Future Endpoints:**  
Using the intersection data, a forecasting model (Prophet) was applied to predict the future endpoints of the shape after learning the historical increment pattern.
<img width="989" height="790" alt="5  predicted endpoints" src="https://github.com/user-attachments/assets/a1ed6c7b-6101-4626-a3c2-b1cb12784082" />
