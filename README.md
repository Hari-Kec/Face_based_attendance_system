

# 🏨 Hostel Management & Face Recognition Attendance System

A complete student hostel management and attendance solution built using **Node.js**, **Express**, **MongoDB**, and **Python OpenCV face recognition**. This system allows for student registration, leave tracking, and automated attendance using real-time facial recognition.

---

## 📦 Features

### 🧠 Face Recognition Attendance (Python)

* Capture and register student face images
* Train model using OpenCV (LBPH Face Recognizer)
* Real-time face recognition and attendance logging
* Attendance saved in Excel format (`.xlsx`)
* Password-protected profile saving
* GUI built with Tkinter
* Wi-Fi SSID check to restrict unauthorized access

### 🌐 Hostel Leave Management (Node.js)

* Register/Login students
* Apply and approve leave requests
* Admin dashboard with student and leave tracking
* EJS-based UI templates for rendering pages
* Data stored using MongoDB

---

## 🛠️ Tech Stack

| Module          | Tech Used                                    |
| --------------- | -------------------------------------------- |
| Backend         | Node.js, Express.js, MongoDB                 |
| Frontend        | EJS Templates                                |
| Face Attendance | Python, OpenCV, Tkinter, Pandas              |
| Storage         | MongoDB (leave data), CSV/Excel (attendance) |

---

## 🗂 Project Structure

```
    <-- Node.js backend (package.json)
/Face_based_attendance_system     <-- Python face recognition (main.py)
├── TrainingImage/
├── TrainingImageLabel/
├── StudentDetails/
├── Attendance/
```

---

## ⚙️ Installation

### 🧠 Face Recognition Setup (Python)

1. Install Python packages:

```bash
pip install opencv-python opencv-contrib-python numpy pandas pillow openpyxl
```

2. Ensure Tesseract OCR and Haar Cascade XML is available:

* `haarcascade_frontalface_default.xml` should be in the root directory.

3. Run the face attendance GUI:

```bash
python main.py
```

### 🌐 Hostel Management System Setup (Node.js)

1. Navigate to backend directory:

```bash
cd hostel_management
npm install
```

2. Start the server:

```bash
npm start
```

3. Access the app on:

```
http://localhost:3000
```

---

## 📈 Workflow

1. **Admin registers a student** in the web app.
2. Student face is registered using the Python GUI.
3. Trained model is saved locally (`Trainner.yml`).
4. During attendance, face recognition matches and logs entry with timestamp.
5. Leave applications are managed separately via the web dashboard.

---

## 📄 License

```
Apache License 2.0

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0
```

---

## 🤝 Contributions

Feel free to fork this repo and open pull requests to improve UI, database integration, or add biometric modules.


