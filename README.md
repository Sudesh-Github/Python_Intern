# Virtual Android System Simulation and Backend Integration

This project contains four tasks: Backend Development, Database Management, Virtual Android System Simulation, and Basic Networking. Follow the instructions below to set up and run each task.

---

## Task 1: Backend Development

### Description
A Python-based API built using Flask with endpoints for managing app details.

### Features
- `POST /add-app`: Add app details to the database.
- `GET /get-app/{id}`: Retrieve app details by ID.
- `DELETE /delete-app/{id}`: Remove an app by ID.

### Setup Instructions
1. **Run the API**:
   ```bash
   python app.py
   
2. **Endpoints**:
    - `Add an app`: POST http://127.0.0.1:5000/add-app
    - `Retrieve an app`: GET http://127.0.0.1:5000/get-app/<id>
    - `Delete an app`: DELETE http://127.0.0.1:5000/delete-app/<id>


## Task 2: Database Management
### Description
SQLite database designed to store app details and integrated with the API.

## Database Schema
# Fields:
  app_id (Primary Key, Auto-Increment)
  app_name (Text)
  version (Text)
  description (Text)
  
Setup Instructions:
1. Create the Database: Run the database_setup.py script:
   ```bash
   python database_setup.py
Sample Data: The script pre-populates the database with sample app details for testing.

Integration: The Flask API (Task 1) automatically interacts with this database.


### Task 3: Virtual Android System Simulation
## Description
A Python script that simulates a virtual Android system using an emulator. It can:

  Launch a virtual device.
  Install a sample APK.
  Retrieve and log system information.
  
# Prerequisites
Android Studio:
Install and configure Android Studio.
Ensure emulator and adb are in the system's PATH.

Sample APK:
Download an APK file (e.g., sample-app.apk) and note its location.
Setup Instructions
Edit Script Configuration: Update paths in the script:

ANDROID_EMULATOR_PATH = "/path/to/emulator"
ADB_PATH = "/path/to/adb"
VIRTUAL_DEVICE_NAME = "Pixel_4_API_30"
APK_FILE_PATH = "/path/to/sample-app.apk"

1. **Run the Script**:
    ```bash
    python virtual_android.py

Expected Output:

The virtual device launches.
The APK is installed.
System information is logged.



