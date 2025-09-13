# **AI-Driven Video Doorbell & App**

<img src="https://github.com/user-attachments/assets/64f4779e-6d94-4b91-859b-e068ba9318a2" width="400">

**Intelligent doorbell system** designed to help home-workers avoid interruptions during video calls. Captures images of visitors, recognises familiar faces with computer vision, and allows the user to interact via a mobile app – all without leaving their desk. 

Developed as part of **A Level Computer Science** coursework and awarded **97%**.  

📹 [Watch the video](https://www.youtube.com/watch?v=hvcWZEq3k6o)  
📄 [Download SmartBell NEA Report](https://orlandoalexander.wordpress.com/wp-content/uploads/2022/10/smartbell-report.docx)
---

## 🛠 Tech Stack

- **Hardware**: Raspberry Pi, camera, speaker, doorbell button  
- **Software**: Python, OpenCV (face recognition), Flask (mobile app backend)  
- **Tools**: Notifications, pre-recorded audio messages, image logging  

---

## 📝 Project Overview

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


**This project was **completed** as part of A Level Computer Science and was awarded 97%.**

<img src="images/image.jpeg" width="400">

For the coursework component of my Computer Science A Level, I wanted to create a project which was genuinely useful. One day I was talking with a family friend who, during COVID, worked mainly from home. She mentioned that often her work calls would get interrupted by people ringing the doorbell, making it hard to stay focused and professional. So, I made it my mission to solve her problem!

Over the course of many months, I designed, developed, tested and refined my solution - and here, in this post, is the final product of much hard-work!

## **So, what exactly is my solution?**

Simply put, it's a doorbell with a brain. The doorbell itself is essentially a Raspberry Pi with some wires dangling off it: a camera, speaker and a button. When the doorbell is rung, the nifty camera captures a photo of the visitor and, if they're a regular, works out their name with a little bit of computer vision (_OpenCV_). Now, the second aspect of the project: the mobile app. This app allows the user to interact with the doorbell (and whoever is ringing the doorbell during a conference call!) directly from their phone. So when the doorbell is rung, a notification pops up on their phone, along with a picture of the visitor (and their name where possible). And then, without leaving their desk, the busy home-worker can then quickly select a pre-recorded audio message to be played through the doorbell's speaker - perhaps 'Could you leave the shopping by the porch?'. In the case that they're out and about when the doorbell is rung, the app will also store a log of all the visits to their house.

Check out this video below to see the doorbell in action: [Watch the video](https://www.youtube.com/watch?v=hvcWZEq3k6o)


## The Report

This report is COMPREHENSIVE to say the least! It covers the ins and outs my solution, as well as challenges faced along the way; there's also lots of pretty diagrams, so enjoy!



[Download SmartBell NEA Report](https://orlandoalexander.wordpress.com/wp-content/uploads/2022/10/smartbell-report.docx)

<img src="images/screenshot-2022-10-14-at-13.10.06-1.png" width="300">
