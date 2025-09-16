# Eye See You!
## A Real-Time Face Recognition Attendance System
Tired of manual attendance? Worried about "buddy punching" or someone using a photo to clock in? Say goodbye to old-school methods! This project is a smart, secure, and real-time attendance system that uses face recognition and a clever anti-spoofing trick to make sure it's the real you.

## 🚀 Key Features
- Real-Time Attendance: Instantly logs people in or out the moment their face is recognized by the camera.
- Secure Authentication: Users can register their face, log in, and log out using just their face.
- Anti-Spoofing: Our system is smart enough to detect and reject fakes! It can tell the difference between a live person and a photo, video, or even a digital screen.
- Simple & Intuitive: A clean interface makes it easy for new users to register and for existing users to use the system without any hassle.

## 🛠️ Get Started (For the Code-Curious!)
Want to get this up and running? Follow these simple steps.

Prerequisites
1. Python 3.8+

2. A webcam

3. pip (for installing dependencies)

- Installation
  - Clone the project:
    - git clone https://github.com/Silverfang180/Facelogix
    - cd Facelogix
3. Create a virtual environment (highly recommended):
- python -m venv venv
- source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
4. Install the magic ingredients:
- pip install -r requirements.txt
## 🧠 How It Works (The Techy Bit)
Our system is a fusion of computer vision and machine learning. Here’s a quick rundown of the main components:
1. Face Detection
   - Detects faces from the video feed (using MTCNN or Haar Cascade).
   - Draws bounding boxes around faces.

2. Facial Embedding
   - A deep learning model (FaceNet/ArcFace) generates a unique faceprint (vector of numbers).
   - Much more reliable than comparing raw pixels.

3. Anti-Spoofing (The Guard Dog )
   - Runs a liveness check (blink detection, light reflection analysis, etc.).
   - Rejects static images, recorded videos, or masks.

4. Verification & Attendance
   - Compares the live faceprint with the database.
   - If matched → logs user attendance with a timestamp.
   - Supports registration → login → logout workflow.

## 🤝 Contributing
This project is a work in progress, and we'd love for you to join us! Whether you want to fix a bug, improve the anti-spoofing, or add a new feature, feel free to open an issue or submit a pull request. Every contribution helps make this a better and more secure system.


