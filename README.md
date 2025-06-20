# 🐶🐱 Image Classifier: Dog vs Cat

This project uses a Convolutional Neural Network (CNN) built with TensorFlow and Keras to classify grayscale images as either a **Dog** or a **Cat**.

## 📁 Project Structure

- `Img_class.ipynb`: Main Jupyter notebook containing all the code from preprocessing to prediction.
- (Optional) `train_data/` and `test_data/`: Directories containing training and testing images respectively.
- Link for training data https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset

## 🧠 Model Overview

The model is a basic CNN that includes:
- Convolutional layers
- MaxPooling
- Flatten and Dense layers
- Sigmoid activation for binary classification

The model is trained to distinguish between grayscale images of cats and dogs.

## 📊 Workflow

1. **Data Preprocessing**
   - Load grayscale images
   - Resize to uniform `IMG_SIZE`
   - Normalize pixel values (`0–255` ➜ `0–1`)
   - Assign binary labels (0 for Cat, 1 for Dog)

2. **Model Training**
   - Sequential CNN model
   - Binary Crossentropy loss
   - Adam optimizer

3. **Prediction & Visualization**
   - Predicts test data labels
   - Visualizes predictions alongside images using `matplotlib`

## ✅ Sample Output

```python
Predicted: Dog (0.84)
