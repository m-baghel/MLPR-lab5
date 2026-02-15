 Lab 5 – Face Clustering Using Color Features (Spring 2026)

This lab implements face detection and unsupervised clustering using color-based features (Hue and Saturation) extracted from detected faces in an image.

##  Aim of the Experiment
To detect human faces in an image and cluster them into groups using K-Means clustering based on their mean Hue and Saturation values.


##  Concept Used
- Face Detection using OpenCV  
- Color Space Transformation (BGR → HSV)  
- Feature Extraction (Mean Hue & Saturation)  
- Unsupervised Learning using K-Means  
- Data Visualization using Matplotlib  
  

##  Libraries Used

- OpenCV (`cv2`)
- NumPy
- Matplotlib
- Scikit-learn (KMeans)
- SciPy

## Files Used

- `Plaksha_Faculty.jpg` – Group image containing multiple faces  
- `Lab 5-Spring 2026.ipynb` – Jupyter notebook containing implementation  

##  Methodology

1. The input image is read and converted to grayscale.
2. Faces are detected using a Haar Cascade classifier.
3. For each detected face:
   - The face region is converted to HSV color space.
   - Mean Hue and Saturation values are computed.
4. Feature vectors are clustered using **K-Means (k = 2)**.
5. A template face is processed similarly.
6. The template face is compared against cluster centroids.
7. Results are visualized using scatter plots.

## Face Detection Output

> Below is the image showing detected faces with bounding boxes
> <img width="1280" height="854" alt="Total number of face detected are 30" src="https://github.com/user-attachments/assets/ca930707-5013-4cef-ad47-cdaa10d889c7" />
.
> <img width="400" height="400" alt="Shashi Tharoor" src="https://github.com/user-attachments/assets/d755151c-fb0a-4b54-8247-e19299c2a215" />

