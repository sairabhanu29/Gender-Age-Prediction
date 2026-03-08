# Gender-Age-Prediction
Age and Gender Prediction using OpenCV and Deep Learning

---

# README.md for GitHub

```markdown
# Gender and Age Prediction using Deep Learning

## Project Overview
This project implements a **Gender and Age Prediction system** using **Computer Vision and Deep Learning**.  
The system detects a human face from an image and predicts:

- **Gender** → Male / Female
- **Age Range** → One of the predefined age groups

The model uses **pre-trained Convolutional Neural Networks (CNNs)** and OpenCV's **Deep Neural Network (DNN)** module.

---

## Objective
The objective of this project is to estimate the **gender and approximate age group of a person from facial images**, while handling challenges such as:

- Lighting variations
- Facial expressions
- Pose differences
- Partial occlusions

---

## Technologies Used

- **Python**
- **OpenCV**
- **Deep Learning (CNN)**
- **Caffe Models**
- **NumPy**
- **Matplotlib / Seaborn**
- **Jupyter Notebook**

---

## Dataset
The pre-trained models used in this project were trained on the **Adience Dataset**, which contains:

- **26,580 images**
- **2,284 subjects**
- Images captured under **real-world conditions**

Age groups used in the dataset:

```

(0-2)
(4-6)
(8-12)
(15-20)
(25-32)
(38-43)
(48-53)
(60-100)

```

---

## Project Structure

```

Gender-and-Age-Detection
│
├── detect.py
├── Gender_Age_Detection.ipynb
│
├── age_net.caffemodel
├── age_deploy.prototxt
│
├── gender_net.caffemodel
├── gender_deploy.prototxt
│
├── opencv_face_detector.pbtxt
├── opencv_face_detector_uint8.pb
│
├── girl1.jpg
├── girl2.jpg
├── kid1.jpg
├── kid2.jpg
├── man1.jpg
├── man2.jpg
├── woman1.jpg
│
└── README.md

````

---

## Installation

Install the required libraries:

```bash
pip install opencv-python
pip install numpy
pip install matplotlib
pip install seaborn
pip install imutils
````

---

## How the System Works

1. **Face Detection**

   * Uses OpenCV DNN face detector.

2. **Face Extraction**

   * The detected face region is cropped.

3. **Gender Prediction**

   * The face is passed through the **gender CNN model**.

4. **Age Prediction**

   * The face is passed through the **age CNN model**.

5. **Result Display**

   * Bounding box with predicted **Age and Gender** is displayed.

---

## How to Run the Project

### Run using an image

```bash
python detect.py --image girl1.jpg
```

### Run using webcam

```bash
python detect.py
```

Press **Ctrl + C** to stop the webcam detection.

---

## Example Output

The system detects faces and displays predictions like:

```
Gender: Female
Age: 25-32
```

Bounding boxes are drawn around the detected face.

---

## Data Analysis

The Jupyter Notebook also includes:

* Data exploration
* Data visualization
* Feature engineering
* Statistical analysis
* Linear regression example

These analyses help understand prediction patterns and dataset characteristics.

---

## Challenges

Age prediction from facial images is difficult due to:

* Makeup
* Lighting conditions
* Facial expressions
* Image quality
* Occlusion (glasses, masks, hair)

To address this, age prediction is treated as a **classification problem** rather than exact regression.

---

## Applications

This system can be used in:

* Retail customer analytics
* Targeted advertising
* Smart surveillance systems
* Human-computer interaction
* Demographic research

---

## Future Improvements

Possible improvements include:

* Training a custom deep learning model
* Improving age prediction accuracy
* Real-time mobile application deployment
* Integration with web applications
* Using larger and more diverse datasets

---

## Author

**B.Tech – Electronics and Communication Engineering (ECE)**
Data Science Project

---

## License

This project is for **educational purposes only**.

```

---


Example structure:

```

Gender-Age-Prediction
│
├── README.md
├── Gender_Age_Detection.ipynb
├── detect.py
├── models
└── images

```

---

