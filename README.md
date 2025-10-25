# 🧠 TrueSight: Image Authentication using CNNs  

**TrueSight** is a deep learning–based image authentication system designed to detect AI-generated or manipulated human faces.  
Built using **TensorFlow**, **Keras**, and **Flask**, the model classifies images as *real* or *fake* with over **95% accuracy**.  
It includes an interactive web interface for real-time image uploads, predictions, and visual analytics.  

---

## 📸 Project Overview  

- Developed a **Convolutional Neural Network (CNN)** for image authenticity verification.  
- Trained on **190K+ images** from the *Kaggle Real and Fake Face Detection Dataset*.  
- Deployed using **Flask** for web-based predictions.  
- Visualized training performance using **Matplotlib** and **Seaborn**.  
- Supports offline usage and lightweight deployment.  

---

## 🚀 Features  

- 🧠 Real vs. Fake human face detection using CNN  
- ⚡ Lightweight, fast, and offline-capable  
- 📊 Real-time result visualization (accuracy graphs, confusion matrix)  
- 🌐 Flask-based web interface for image uploads and predictions  
- 🔒 Practical use in digital forensics, media verification, and AI security  

---

## 🛠️ Tech Stack  

| Category | Tools & Frameworks |
|-----------|-------------------|
| **Programming Language** | Python 3.10+ |
| **Libraries** | TensorFlow, Keras, NumPy, OpenCV, Matplotlib, Seaborn, Scikit-learn, Pillow |
| **Web Framework** | Flask |
| **Dataset** | Kaggle - Real and Fake Face Detection |
| **Environment** | VS Code / Google Colab |

---

## ⚙️ How to Run the Project in VS Code  

### 🧩 Step 1: Install Prerequisites  
- Install [**VS Code**](https://code.visualstudio.com/)  
- Install [**Python 3.10+**](https://www.python.org/downloads/)  
- Verify installation:  
  ```bash
  python --version
🧱 Step 2: Set Up the Project Folder
arduino
Copy code
TrueSight_Project/
│
├── app.py
├── TrueSight.ipynb
├── new_model.h5
├── static/
│   ├── uploads/
│   ├── images/
│   └── style.css
└── templates/
    ├── base.html
    ├── home.html
    ├── upload.html
    └── result.html
⚙️ Step 3: Create a Virtual Environment
bash
Copy code
python -m venv venv
Activate it:

Windows: venv\Scripts\activate

Mac/Linux: source venv/bin/activate

📦 Step 4: Install Dependencies
bash
Copy code
pip install tensorflow keras numpy opencv-python matplotlib seaborn scikit-learn flask pillow
(Optional for GPU acceleration)

bash
Copy code
pip install tensorflow-gpu
📓 Step 5: Run and Test the Model
Open TrueSight.ipynb in VS Code.

Run the notebook to verify model training.

Save trained weights:

python
Copy code
model.save("new_model.h5")
🌐 Step 6: Launch Flask Web App
Ensure this line exists in app.py:

python
Copy code
model.load_weights('new_model.h5')
Run the app:

bash
Copy code
python app.py
Open your browser at → http://127.0.0.1:5000/

✅ Upload an image → Get prediction → View confidence score and result visualization.

🧮 Step 7: Common Debugging Tips
Issue	Fix
ModuleNotFoundError	Install missing package via pip install <package>
Model not loading	Verify correct path to new_model.h5
Flask not starting	Try different port: python app.py --port 8080
Image upload error	Ensure static/uploads/ folder exists

📊 Results
Achieved 95%+ classification accuracy on test data

Validated using confusion matrix, ROC curve, and performance graphs

Demonstrated real-time prediction with user-friendly web interface
