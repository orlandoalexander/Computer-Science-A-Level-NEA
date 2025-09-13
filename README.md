# AI-Driven Video Doorbell & App

<img src="https://github.com/user-attachments/assets/64f4779e-6d94-4b91-859b-e068ba9318a2" width="400">

**AI-driven video doorbell and mobile app** designed to help home-workers avoid interruptions during video calls. Captures images of visitors, recognises familiar faces with computer vision, and allows the user to interact via a mobile app – all without leaving their desk. 

Coursework project for **A Level Computer Science** awarded **97%**.  

📄 [Download Project Report](https://orlandoalexander.wordpress.com/wp-content/uploads/2022/10/smartbell-report.docx)
📹 [Watch Demo Video ](https://www.youtube.com/watch?v=hvcWZEq3k6o)  


## 🛠 Tech Stack

- **Hardware**: Raspberry Pi 4, Monk Makes Speaker Module, Raspberry Pi Camera Module V1
- **Software**: Python Kivy (movile app frontend), Flask (mobile app backend), OpenCV (image processing), face_recognition (deep learning-based face recognition),


## 📝 Project Overview

For my A Level Computer Science coursework, I wanted to create a project that was genuinely useful. During COVID, a family friend working from home mentioned that her video calls were frequently interrupted by visitors ringing the doorbell, making it difficult to stay focused and professional. I decided to solve this problem with an intelligent, AI-powered solution.  

Over several months, I designed, developed, tested, and refined a fully functional system *SmartBell*. Here is the final product of that hard work:

### What is SmartBell?

SmartBell is an AI-driven video doorbell and mobile app. At its core, a Raspberry Pi equipped with a camera, speaker, and button captures an image of any visitor. If the visitor is familiar, the system recognises them using **deep learning-based face recognition** via the Python `face_recognition` library.  

The mobile app allows the user to interact with the doorbell in real-time. When the doorbell is rung, a notification appears on the user’s phone with a photo of the visitor and, where possible, their name. The user can then play a pre-recorded audio message through the doorbell’s speaker—for example, *“Could you leave the shopping by the porch?”*—without leaving their desk. If the user is away, the app logs all visits, storing images and timestamps for easy review.


### 1. Visitor Detection
- Button press triggers Raspberry Pi camera  
- Captures image of the visitor  
- Detects faces using **OpenCV Haar cascades**  
- Prepares image for **face recognition**

### 2. Mobile App Interaction
- Sends notification to the user’s phone with visitor image and name  
- Allows pre-recorded messages to be played remotely  
- Logs visits when the user is unavailable  

### 3. Face Recognition (ML Component)
- Computes **face encodings** for each detected face  
- Compares encodings to a stored database of known visitors  
- Detects and identifies visitors in real-time  
- Updates the database with new faces to improve recognition accuracy  

### 4. Logging & Notifications
- Stores visitor images and timestamps in a cloud database  
- Sends notifications even when the user is away  
- Provides an easy-to-review visitor history for the user

- 

For the coursework component of my Computer Science A Level, I wanted to create a project which was genuinely useful. One day I was talking with a family friend who, during COVID, worked mainly from home. She mentioned that often her work calls would get interrupted by people ringing the doorbell, making it hard to stay focused and professional. So, I made it my mission to solve her problem!

Over the course of many months, I designed, developed, tested and refined my solution - and here, in this post, is the final product of much hard-work!

### **So, what exactly is my solution?**

Simply put, it's a doorbell with a brain. The doorbell itself is essentially a Raspberry Pi with some wires dangling off it: a camera, speaker and a button. When the doorbell is rung, the nifty camera captures a photo of the visitor and, if they're a regular, works out their name with a little bit of computer vision (_OpenCV_). Now, the second aspect of the project: the mobile app. This app allows the user to interact with the doorbell (and whoever is ringing the doorbell during a conference call!) directly from their phone. So when the doorbell is rung, a notification pops up on their phone, along with a picture of the visitor (and their name where possible). And then, without leaving their desk, the busy home-worker can then quickly select a pre-recorded audio message to be played through the doorbell's speaker - perhaps 'Could you leave the shopping by the porch?'. In the case that they're out and about when the doorbell is rung, the app will also store a log of all the visits to their house.


### 1. Visitor Detection
- Button press triggers Raspberry Pi camera  
- Captures image of visitor  
- Uses **OpenCV face recognition** to identify known visitors  

### 2. Mobile App Interaction
- Sends notification to the user’s phone with visitor image and name  
- Allows pre-recorded messages to be played through the doorbell speaker  
- Logs all visits when user is unavailable  

### 3. Face Recognition
- Detects and identifies visitors in real-time  
- Maintains a database of familiar faces for faster recognition  
- Uses image preprocessing to improve recognition accuracy  

### 4. Logging & Notifications
- Stores all visitor images and timestamps  
- Sends notifications even when user is away from home  
- Allows easy review of visitor history
