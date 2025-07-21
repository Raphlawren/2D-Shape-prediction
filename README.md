<img width="1162" height="699" alt="3  intersection lines" src="https://github.com/user-attachments/assets/02ef6f28-9ec7-4e2d-97b9-f8d9709f29b9" /># 2D-Shape-prediction

This is a paper in progress. Below is a rough overview of what has been done so far.

This project explores forecasting the evolution of a 2D shape over time using radial sampling and time-series prediction techniques.

I manually created circle expanded each year slightly to simulate shape evolution over time. 
<img width="1200" height="729" alt="1  CIrcular layers" src="https://github.com/user-attachments/assets/5e00029c-4d5a-4a9a-9660-e702768e09e9" />


I calculated the centroid of the first year shape and extracted the geometry for that point and created a radial line from the point to cover the shape. These lines extended outward in 1-degree increments to cover the full circular boundary of the shapes
<img width="1179" height="724" alt="2  Radial Line" src="https://github.com/user-attachments/assets/3a994d32-afe9-4445-b1a8-5e28ccd5fbb9" />

I performed an intersection of the shapes with the the radial lines.
<img width="1162" height="699" alt="3  intersection lines" src="https://github.com/user-attachments/assets/9c9c040e-4e25-4e71-a7d8-5ff84fd1ebfc" />

Then i predicted the future endpoint of the shape after the model has understood the pattern and the increment. 
<img width="989" height="790" alt="5  predicted endpoints" src="https://github.com/user-attachments/assets/a1ed6c7b-6101-4626-a3c2-b1cb12784082" />
