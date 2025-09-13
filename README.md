# AI-Driven Video Doorbell & Mobile App

<img src="https://github.com/user-attachments/assets/64f4779e-6d94-4b91-859b-e068ba9318a2" width="400">
<img width="1080" height="834" alt="nea-cover2" src="https://github.com/user-attachments/assets/efae47b3-ac67-4718-8656-620909eb4169" />

**AI-driven video doorbell and mobile app** designed to help home-workers avoid interruptions during video calls. Captures images of visitors, recognises familiar faces with computer vision, and allows the user to interact via a mobile app – all without leaving their desk. 

Coursework project for **A Level Computer Science** awarded **97%**.  

📄 [Download Project Report](https://orlandoalexander.wordpress.com/wp-content/uploads/2022/10/smartbell-report.docx)<br>
📹 [Watch Demo Video ](https://www.youtube.com/watch?v=hvcWZEq3k6o)<br><br>


## 🛠 Tech Stack

- **Hardware**: Raspberry Pi 4, Monk Makes Speaker Module, Raspberry Pi Camera Module V1
- **Software**: OpenCV (image processing), face_recognition (deep learning-based face recognition), Python Kivy (movile app frontend), Flask (mobile app backend)<br><br>


## 📝 Project Overview

For my A Level Computer Science coursework, I wanted to create a project that was genuinely useful. During COVID, a family friend working from home mentioned that her video calls were frequently interrupted by visitors ringing the doorbell, making it difficult to stay focused and professional. I decided to solve this problem with an intelligent, AI-powered solution.  

Over several months, I designed, developed, tested, and refined a fully functional system **SmartBell**. Here is the final product of that hard work:

### What is SmartBell?

SmartBell is an AI-driven video doorbell and mobile app. At its core, a Raspberry Pi equipped with a camera, speaker, and button captures an image of any visitor. If the visitor is familiar, the system recognises them using **deep learning-based face recognition** via the Python `face_recognition` library.  

The mobile app allows the user to interact with the doorbell in real-time. When the doorbell is rung, a notification appears on the user’s phone with a photo of the visitor and, where it is known, their name. The user can then play a pre-recorded audio message through the doorbell’s speaker without leaving their desk, for example, *“Could you leave the shopping by the porch?”*. If the user is away, the app logs all visits, storing images and timestamps for easy review.


### Visitor Capture & Detection
- Button press triggers Raspberry Pi camera to capture visitor image  
- Detects faces using **OpenCV Haar cascades**  
- Sends notification to the user’s phone with visitor image and name (if recognised)  

### AI-Powered Face Recognition
- Computes **face encodings** for each detected face using `face_recognition`  
- Compares encodings against a stored database of known visitors  
- Identifies visitors in real-time and updates database with new faces for improved accuracy  

### Mobile App 
- Notifies user when the doorbell is rung and displays visitor image and name (if available)  
- Plays pre-recorded messages remotely via Raspberry Pi speaker  
- Logs visits when the user is unavailable  

### Cloud Logging & Notifications
- Stores visitor images and timestamps in a secure cloud database  
- Sends notifications even when the user is away from home  
- Provides an easy-to-review history of all visits<br><br>

## ⚙️ System Design

### Mobile App
<img width="708" height="559" alt="Mobile App Screenshot" src="https://github.com/user-attachments/assets/25f52962-6f74-4fb4-bddc-81452e23cd09" />

### Backend Server
<img width="607" height="733" alt="Backend Server Screenshot" src="https://github.com/user-attachments/assets/f62c6ccd-010c-498e-819b-58c3e6431137" />

### Raspberry Pi
<img width="764" height="294" alt="Raspberry Pi Screenshot" src="https://github.com/user-attachments/assets/430a3b4b-56ce-46c2-93c0-4ba8a3f84f16" />

