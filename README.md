# Face Authentication Login System

This project implements a face authentication login system using Flask, OpenCV, and face_recognition.

## Prerequisites

Make sure you have the following installed on your system:
- Python 3.8 or later
- pip

## Setup Instructions

1. **Clone the Repository**

```sh
git clone https://github.com/Dana7afez/face-authentication-login-system.git
cd face-authentication-login-system
```

2. **Create and Activate a Virtual Environment**

```sh
# Create a virtual environment
python -m venv venv

# Activate the virtual environment
.\venv\Scripts\Activate.ps1  # For Windows PowerShell
# source venv/bin/activate  # For Linux/Mac
```

3. **Install Required Packages**

```sh
pip install --upgrade pip
pip install setuptools  # Ensure setuptools is installed
pip install -r requirements.txt
```

4. **Set Up the Face Recognition Models**

Download the face recognition models and place them in the specified path. Update the `FACE_RECOGNITION_MODEL_PATH` environment variable in the `run_app.py` file to point to the models.

5. **Run the Application**

```sh
cd backend
python run_app.py
```

## Usage

### Register a User

1. Go to the registration page (`/register`).
2. Enter a name and take a selfie to register.
3. Ensure the user is registered successfully.

### Login

1. Go to the login page (`/login`).
2. Take a selfie to log in.
3. Ensure the login is successful for the registered user.

## Testing

### Clear Data

To clear the existing user data and start fresh, delete the `users.db` file located in the `backend/database` directory.

```sh
cd backend/database
del users.db  # For Windows
# rm users.db  # For Linux/Mac
```

### Test Authorized and Unauthorized Access

1. Register a known user.
2. Test login with the registered user (authorized access).
3. Test login with an unregistered user (unauthorized access).

## Dependencies

- Flask>=3.1.0
- opencv-python>=4.11.0.86
- face-recognition>=1.3.0
- sqlalchemy>=2.0.38
- cryptography>=44.0.1
- flask-ngrok>=0.0.25
- face_recognition_models @ file:///C:/Users/danah/Desktop/ATRS/face-authentication-login-system/face_recognition_models-master/face_recognition_models-master

## License

This project is licensed under the MIT License.