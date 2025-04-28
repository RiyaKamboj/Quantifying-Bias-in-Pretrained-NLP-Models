# Quantifying Bias in Pretrained NLP Models

## 📜 Project Description
This project focuses on analyzing and mitigating biases present in popular pretrained word embeddings such as **Word2Vec**, **GloVe**, and **FastText**.  
We use **WEAT (Word Embedding Association Test)** to quantify the level of bias across dimensions like gender, race, and religion.  
We also implement debiasing techniques — **HardWEAT** and **SoftWEAT** — to reduce these biases, and re-evaluate the embeddings post-debiasing to measure improvements.

The entire workflow is designed to be reproducible in Google Colab, with all dependencies, datasets, and custom modules provided.

---

## 👩‍💻 Team Members
| Name            |      
|-----------------|
| Apoorva Jindal  |  
| Riya Kamboj     |  

---

## 👨‍🏫 Supervisor
- **Name:** Sakshi  
- **E-Code:** E16561

---

## 📂 Project Structure
- **Datasets/**: Contains the pretrained embeddings and evaluation datasets (after extraction).
- **Classes/**: Custom Python classes, including `Word_Embedding` for loading and manipulating embeddings.
- **Evaluation/**: Scripts for performing bias evaluation tasks such as WEAT and sentiment analysis.
- **Utils/**: Helper functions and methods needed for dataset preparation and debiasing.

---

## 🚀 How to Run
1. **Upload Required Files**:  
   - Upload `folders.zip` (contains Classes/, Evaluation/, Utils/ folders) to Colab.
   - Download and extract `datasets.zip` automatically using the provided script.

2. **Install Dependencies**:  
   Run the provided cell to install exact versions of `numpy`, `tensorflow`, `gensim`, `nltk`, `matplotlib`, and others.  
   Also install `keras_preprocessing` to fix any compatibility issues.

3. **Initialize Environment**:  
   Import the necessary modules and set up visualization preferences.

4. **Select Embedding**:  
   Choose among Word2Vec, GloVe, or FastText for bias analysis.

5. **Bias Quantification (WEAT)**:  
   Measure initial bias levels using WEAT.

6. **Debias Embeddings**:  
   Apply HardWEAT and SoftWEAT debiasing methods.

7. **Re-evaluate**:  
   Perform WEAT again to compare the bias levels before and after debiasing.

---

## 🛠 Technologies Used
- Python 3.10+
- TensorFlow 2.12
- NumPy 1.23
- Pandas 1.5
- Gensim 4.3
- Scikit-learn 1.2
- NLTK 3.8
- Matplotlib & Seaborn for visualization
- Google Colab environment

---

## 📈 Results
The project demonstrates that both **HardWEAT** and **SoftWEAT** successfully reduce biases in pretrained word embeddings, as quantified by lower WEAT d-values after debiasing.

---

## 📋 License
This project is for academic purposes only.
