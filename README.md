# Siamese Neural Network for Facial Recognition

This project implements a **Facial Recognition System** using Siamese Neural Networks (SNN). The model is trained to compare two facial images and determine if they belong to the same person. This approach is widely used for applications such as face authentication, access control, and more.

---

## Features
- **One-shot learning:** Identifies faces with limited training data.
- **Custom dataset creation:** Train the model with your own images.
- **High accuracy:** Optimized model for robust performance.

---

## Project Description

Facial recognition is achieved using **Siamese Neural Networks**, a deep learning architecture designed to find similarity between two inputs. Unlike traditional classification models, SNNs focus on learning a distance metric to measure the similarity between facial images.

Key steps:
1. **Data Preparation:** Images are preprocessed and paired as matching or non-matching pairs.
2. **Model Training:** The SNN is trained to minimize the contrastive loss, which measures the distance between embeddings of paired images.
3. **Real-time Recognition:** After training, the model is used to verify or identify faces in real time.

**Model Accuracy:** The system achieves an accuracy of approximately **92%** on the test set, with a false positive rate of 5% for challenging datasets.

---

## Dataset

The dataset for this project was prepared **manually**. It consists of facial images of multiple individuals, carefully labeled and organized for training and testing.

### Dataset Preparation
1. **Collect images:** Capture or gather facial images for each individual.
2. **Organize the dataset:** Save the images in folders, where each folder corresponds to a specific individual:
   ```
   dataset/
   ├── person1/
   │   ├── img1.jpg
   │   ├── img2.jpg
   ├── person2/
   │   ├── img1.jpg
   │   ├── img2.jpg
   ```
3. **Generate image pairs:** Create pairs of images for training:
   - Positive pairs: Two images of the same person.
   - Negative pairs: Images of different people.

---

## Requirements

Install the required dependencies using the following command:
```bash
pip install -r requirements.txt
```

### Key Dependencies
- TensorFlow
- Keras
- NumPy
- OpenCV
- Matplotlib

---

## How to Use

### Step 1: Clone the Repository
```bash
git clone https://github.com/your-username/snn-facial-recognition.git
cd snn-facial-recognition
```

### Step 2: Place Your Dataset
Place your prepared dataset in the `dataset/` directory as described above.

### Step 3: Train the Model
Run the training script to train the Siamese Neural Network and save the trained model:
```bash
python train_snn.py
```

### Step 4: Real-time Recognition
Use the real-time recognition script to test the model with new images:
```bash
python realtime_recognition.py
```

### Step 5: Verify Results
Upload facial images or use a webcam to test the system's accuracy in recognizing individuals.

---

## File Structure
- `train_snn.py`: Script for training the Siamese Neural Network.
- `realtime_recognition.py`: Script for real-time facial recognition using the trained model.
- `snn_model.h5`: Saved model file after training.
- `requirements.txt`: Dependencies for the project.

---

## Contributions
Feel free to contribute to this project by submitting issues or pull requests. Suggestions for improving the model or optimizing the pipeline are always welcome!

---

## Author
**Akhand Pratap Singh**  
Passionate about deep learning and computer vision. 😊

---
