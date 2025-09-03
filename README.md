# Bell's Palsy Detection and Severity Grading using Machine Learning

This repository contains a machine learning project designed to **detect the presence of Bell's Palsy** and **grade its severity** from facial images and video streams.

---

## 📑 Table of Contents
- [What is Bell's Palsy?](#-what-is-bells-palsy)
- [Project Objective](#-project-objective)
- [Our Approach](#-our-approach)
- [Impact and Results](#-impact-and-results)
- [Technology Stack](#-technology-stack)
- [How to Use](#-how-to-use)
- [Image Samples](#-image-samples)

---

## 🧠 What is Bell's Palsy?

Bell's Palsy is a neurological condition characterized by the sudden onset of weakness or paralysis in the muscles on one side of the face.  
This condition occurs when the **seventh cranial nerve**, which controls facial muscles, becomes inflamed or compressed. While the exact cause is often unknown, it is frequently linked to viral infections.

**Key symptoms include:**
- Facial drooping on one side, including the eyebrow and mouth  
- Difficulty making facial expressions (e.g., smiling, closing an eye)  
- Drooling from one side of the mouth  
- Altered sense of taste  
- Pain around the jaw or behind the ear on the affected side  

The condition is typically **temporary**, with most individuals showing significant improvement within a few weeks, and full recovery within six months.  
➡️ Early detection and monitoring are crucial for managing symptoms and tracking recovery progress.

---

## 🎯 Project Objective

The primary goal of this project is to **utilize machine learning** to automatically **grade the severity of Bell's Palsy** from images and videos.  
This can serve as a valuable tool for:
- Assisting in initial diagnosis  
- Monitoring a patient's recovery progress over time  

---

## 🔬 Our Approach

Our methodology involves the following steps:

1. **Feature Extraction**  
   - Used **MediaPipe** to extract key facial landmarks.  
   - Precisely masked the **mouth region** to isolate the most indicative features.  

2. **Dataset**  
   - Collected a dataset of **1000+ images**.  
   - Preprocessed and vectorized the dataset for model training.  

3. **Modeling**  
   - Trained a **Random Forest model** on the vectorized dataset.  
   - Classified images as "healthy" or "Bell’s Palsy affected."  

4. **Evaluation**  
   - Model performance evaluated on **video frames**.  
   - Calculated a **severity score** as:  

     ```
     severity = (frames classified as affected) / (total frames)
     ```  

   - This provides a **quantitative measure** of the condition's severity.  

---

## 📊 Impact and Results

- Achieved **90% accuracy** on still images.  
- Next phase: **Real-time video analysis** for immediate feedback and continuous monitoring.  

---

## ⚙️ Technology Stack

- **Python**  
- **OpenCV** → Image & video processing  
- **MediaPipe** → Facial landmark detection  
- **Scikit-learn** → Random Forest model  
- **NumPy** → Numerical operations  

---

## 🚀 How to Use

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/bells-palsy-detection.git
   cd bells-palsy-detection
