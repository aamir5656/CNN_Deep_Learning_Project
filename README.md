#  Dog vs Cat Classification (CNN)

This project is about classifying **dogs and cats** using a **Convolutional Neural Network (CNN)** built with **TensorFlow/Keras**.  
The dataset used in this project was **downloaded from Kaggle**.

---

##  About the Project
Convolutional Neural Networks (CNNs) are special deep learning models used for image classification.  
They automatically learn important features from images like edges, shapes, and textures.  

In this project, our CNN model learns how to differentiate between dog and cat images.

---

##  How It Works
1. **Data Preprocessing**  
   - Images are resized to 64x64 pixels.  
   - Pixel values are normalized (0–1 range).  
   - Data augmentation (rotation, zoom, flip) is used to avoid overfitting.  

2. **CNN Model**  
   - Convolution + MaxPooling layers extract features.  
   - BatchNormalization improves training.  
   - Dropout prevents overfitting.  
   - Dense layers make the final decision.  
   - Output layer uses **sigmoid activation** for binary classification.  

3. **Training**  
   - Loss function: `binary_crossentropy`  
   - Optimizer: `Adam (lr=0.0001)`  
   - Callbacks: `EarlyStopping` and `ModelCheckpoint`  

4. **Prediction**  
   - A new image can be given to the model.  
   - Model predicts if it’s a **dog** or a **cat** with probability.  

---

##  Dataset
- Dataset: [Kaggle Dogs vs Cats](https://www.kaggle.com/c/dogs-vs-cats/data)  
- Thousands of labeled images of dogs and cats.  
- Divided into **training** and **test** sets.  

---

##  Results
Example output:
```
Predicted class: dog  
Probability of being dog: 0.8723
```


## 📜 Note

This project uses the [Cats and Dogs Dataset](https://www.kaggle.com/datasets/tongpython/cat-and-dog).  
If you are running this notebook outside Kaggle, please download the dataset manually and update the path.

And also remember this 
- Dataset belongs to Kaggle.  
- This project is for **educational purposes** only.  
