# Face Authentication Login System

## Project Description
A face-based authentication system that allows users to register and log in using their facial features. The system captures a user's face, stores the encoding, and uses it for authentication during login attempts.

## Features
- User Registration with Face Capture
- User Login with Face Recognition
- Real-time Video Feed for Face Capture
- Flask-based Web Application
- SQLite Database for User Data Storage

## Prerequisites
- Python 3.8 or higher
- Virtual Environment (venv)
- Webcam for Face Capture

## Installation Instructions
1. Clone the repository:
   ```sh
   git clone https://github.com/your_username/face-authentication-login-system.git
   cd face-authentication-login-system
   ```

2. Create and activate a virtual environment:
   ```sh
   python -m venv venv
   .\venv\Scripts\Activate.ps1
   ```

3. Install required packages:
   ```sh
   pip install -r requirements.txt
   ```

4. Set the environment variable for the face recognition models:
   ```sh
   $env:FACE_RECOGNITION_MODEL_PATH="C:\Path\To\face_recognition_models\models"
   ```

5. Run the Flask application:
   ```sh
   cd backend
   python app.py
   ```

## Usage Instructions
- Open the web browser and navigate to `http://127.0.0.1:5000/`
- Register a new user by providing a username and capturing a selfie
- Log in with the registered user by capturing a selfie
- The system will authenticate the user based on the stored face encoding

## License
This project is licensed under the MIT License.

## Author
Developed by Dana Hafez

## Acknowledgments
- [Face Recognition Library](https://github.com/ageitgey/face_recognition)
- [Flask Web Framework](https://flask.palletsprojects.com/)