# Plant Disease Prediction (Flask App)

A simple Flask web application that predicts plant diseases from leaf images using a PyTorch model.  
Upload an image → the model analyzes it → the app returns the predicted disease.

---

## 📁 Project Structure

Flask Deployed App/
│── app.py
│── CNN.py
│── requirements.txt
│── plant_disease_model_1.pt (added manually)
│── static/
│── templates/
│── venv/ (ignored in git)



---

## ⚙️ Setup & Installation

### 1. Install Python 3.8
The project dependencies were built for Python 3.8.  
Download from: https://www.python.org/downloads/release/python-3810/

> Make sure to check **"Add Python to PATH"** during installation.

---

### 2. Create a Virtual Environment

Open PowerShell in the project folder:

py -3.8 -m venv venv



Activate it:

venv\Scripts\activate



---

### 3. Install Dependencies

pip install -r requirements.txt



This installs Flask, Torch, and other required packages.

---

### 4. Add the Model File

Download the model:

plant_disease_model_1.pt [here](https://drive.google.com/drive/folders/1VRIUNjAnrZpxUjuyx14xN3TVSUz-DtrK?usp=sharing)


Place it in the same folder as `app.py`.

---

## ▶️ Run the App

Start the Flask server:

python app.py



The app will run at:

http://127.0.0.1:5000/



You can open it in any browser.

---

## 📝 Notes

- Works on CPU — no GPU required.
- venv and model files are ignored using `.gitignore`.
- For `/` and `/index`, routing is already handled with:

@app.route('/')
@app.route('/index')




- Make sure the model file is present before starting the server.


