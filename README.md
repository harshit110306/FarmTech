
# 🌾 **FarmTech – Your Smart Farming Assistant**

FarmTech is a modern, AI-powered web application designed to empower farmers with **data-driven insights** for improved agricultural decision-making. It seamlessly integrates **machine learning**, **real-time weather forecasting**, and an **intelligent AI chatbot** to provide actionable guidance on crop selection, climate conditions, and general farming knowledge.

---

## 🚀 **Features**

### 🔐 **User Authentication**

Secure registration and login system to ensure protected access for all users.

### 🌱 **Crop Recommendation System**

Predicts the most suitable crop based on a trained machine learning model using parameters like:

* Nitrogen (N), Phosphorus (P), Potassium (K)
* Temperature
* Humidity
* Soil pH
* Rainfall

### ☁️ **Weather Forecasting**

Comprehensive real-time weather information:

* **Current Weather**: Temperature, humidity, pressure, visibility, sunrise/sunset
* **Hourly Forecast**: Detailed next 24 hours
* **Weekly Forecast**: Weather trends for the upcoming week

### 🤖 **AgroAI – Intelligent Farming Chatbot**

Your personal farming assistant capable of:

* Answering predefined agricultural FAQs
* Extracting information from a **PDF knowledge base**
* Using **OpenAI GPT** to respond to complex farming and crop-related queries

---

## 🛠️ **Technology Stack**

### **Backend**

* Python
* Flask

### **Database**

* MongoDB

### **Machine Learning**

* Scikit-learn
* Pandas
* NumPy

### **External APIs**

* **OpenWeatherMap API** – Real-time weather data
* **OpenAI API** – Chatbot intelligence

### **Frontend**

* HTML, CSS, JavaScript (Flask templating)

---

## 📁 **Project Structure**

```
FarmTech/
├── .venv/                  # Virtual environment
├── templates/              # Frontend HTML templates
│   ├── reg.html
│   ├── login.html
│   └── home.html
├── app.py                  # Main Flask app and routing
├── chat.py                 # AgroAI chatbot logic
├── d_weather.py            # Daily/hourly weather functionality
├── w_weather.py            # Weekly weather functionality
├── soil.py                 # Crop recommendation model logic
├── crop_data.csv           # Dataset for ML model
├── Chat.pdf                # Knowledge base for chatbot
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

---

## ⚙️ **Setup & Installation**

Follow these steps to run FarmTech locally.

### **1. Prerequisites**

* Python 3.8+
* MongoDB Atlas (or local MongoDB)
* API keys for:

  * OpenWeatherMap
  * OpenAI

---

### **2. Clone the Repository**

```bash
git clone https://github.com/harshit110306/FarmTech.git
cd FarmTech
```

---

### **3. Create & Activate Virtual Environment**

#### **Windows**

```bash
python -m venv .venv
.venv\Scripts\activate
```

#### **macOS / Linux**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

---

### **4. Install Dependencies**

Replace `requirements.txt` content with:

```
Flask
pymongo
scikit-learn
pandas
numpy
requests
PyPDF2
openai
gunicorn
```

Then run:

```bash
pip install -r requirements.txt
```

---

### **5. Configure Environment Variables**

Update the following files with your credentials:

#### **`app.py`** – MongoDB URI

```python
uri = "mongodb+srv://<user>:<password>@<cluster-uri>/?retryWrites=true&w=majority"
```

#### **`d_weather.py` and `w_weather.py`** – OpenWeatherMap API Key

```python
API_KEY = "YOUR_OPENWEATHERMAP_API_KEY"
```

#### **`chat.py`** – OpenAI API Key

```python
openai.api_key = "YOUR_OPENAI_API_KEY"
```

---

### **6. Run the Application**

```bash
python app.py
```

The app will run at:

👉 **[http://127.0.0.1:5000](http://127.0.0.1:5000)**

---

## 🧭 **How to Use**

1. **Register** using your name and 10-digit mobile number.
2. **Login** with your credentials.
3. **Crop Recommendation**:

   * Go to **Soil Analysis**, fill in soil/environment values, get instant prediction.
4. **Weather Forecast**:

   * Check daily, hourly, or weekly weather for your location.
5. **AgroAI Chatbot**:

   * Ask farming-related questions and get intelligent responses.

---

## 📌 **Future Enhancements**


* Voice-enabled chatbot
* Integration with IoT soil sensors
* Crop disease detection module
* Mobile app support

---

## 🧑‍🌾 **Contributing**

Contributions are welcome!
Feel free to open issues or submit pull requests.

---

## 📌 **References**

![Alt text](https://github.com/Adi-ADI2005/FarmTech-/blob/f24930532b63dd3113d689388214256a63cc4037/farmtech.png)



[Visit Farmtech ](https://farmtech-1-q7uw.onrender.com/)


## 📜 **License**

This project is licensed under the **MIT License**.

---

