## ML Hand Gesture Recognition
Hand Gesture Recognition is a Python GUI application that uses computer vision and machine learning to recognize Sign Language gestures in real time. 
It supports three core workflows: predicting signs from camera input, translating speech to sign language, and building custom sign datasets. 
The app features a secure login/signup system backed by a local SQLite database, ensuring only registered users can access the recognition tools.

## ✨ Features

🔐 User Authentication — Secure login and signup with SQLite-backed credential storage
🖐️ Sign Prediction — Real-time ISL gesture recognition via webcam
🎙️ Speech to Sign Translation — Convert spoken words into corresponding sign language output
📸 Dataset Creation — Capture and save custom sign images to train or extend the model
🎞️ Animated UI — Smooth GIF animations and a clean tabbed interface built with Tkinter
📊 Excel Export — Export data using xlsxwriter


## 🛠️ Tech Stack
LayerTechnologyGUIPython tkinter, ttkComputer VisionOpenCV (cv2)Image ProcessingPillow (PIL)Data Handlingpandas, numpyDatabaseSQLite3AudioplaysoundExportxlsxwriter

## 📁 Project Structure
ISL-Recognition/
│
├── main.py                  # Entry point — login UI & navigation
├── creating_dataset.py      # Module to capture and save sign images
├── Prediction.py            # Module for real-time sign prediction
├── Reverse_Recognition.py   # Module for speech-to-sign translation
│
├── files/
│   ├── users_info.db        # SQLite database for user credentials
│   └── gif2.gif             # Animated GIF for the main panel
│
└── README.md

## ⚙️ Installation
Prerequisites

Python 3.7+
A working webcam (for sign prediction and dataset creation)
A microphone (for speech translation)

Steps

Clone the repository

bash   git clone https://github.com/your-username/isl-recognition-system.git
   cd isl-recognition-system

Install dependencies

bash   pip install opencv-python pillow pandas numpy playsound xlsxwriter

Create the required directory

bash   mkdir files

Run the application

bash   python main.py

The SQLite database (users_info.db) is created automatically on first launch inside the files/ folder.


## 🚀 Usage

Sign Up — Go to the Sign_up tab, enter a username and password, and click Add User.
Log In — Switch to the Login tab, enter your credentials, and click Login.
Once logged in, the User Panel gives you access to three tools:


## 📦 Modules
🖐️ Predict Sign (Prediction.py)
Opens the webcam and uses a trained model to recognize and display Indian Sign Language gestures in real time.
🎙️ Translate Speech (Reverse_Recognition.py)
Captures spoken input via microphone and maps it to the corresponding ISL sign output.
📸 Create Signs (creating_dataset.py)
Launches a camera interface to capture and label sign images, building a local dataset for model training or extension.

## 🗄️ Database
The app uses a local SQLite database stored at files/users_info.db.
Table: users
ColumnTypeDescriptionnameTEXTUsernamepasssTEXTPassword (plain text)sqltimeTIMESTAMPAccount creation time (auto)

⚠️ Note: Passwords are currently stored in plain text. For production use, consider hashing passwords with bcrypt or hashlib.


## 📸 Screenshots

Add screenshots of your login screen, user panel, and sign prediction window here.

## Author
Aniket Chaudhary
