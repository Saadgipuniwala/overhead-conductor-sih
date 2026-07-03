# Overhead Conductor Fault Detection

Smart grid monitoring and fault detection system using Flask and simulated LoRa communication to monitor pole health, assign maintenance tasks, and visualize fault locations.

**Developed by Team SYNKTRA**

## Repository

https://github.com/Saadgipuniwala/overhead-conductor-fault-detection

## Live Demo

https://overhead-conductor-fault-detection-1.onrender.com

## Local Development

http://localhost:5001

---

## Overview

Smart Voltage Breakage Detection System (LV_AC) is a Flask-based web application developed to monitor the health of low-voltage (LV) AC distribution poles using simulated IoT sensor data.

Pole-mounted sensors equipped with accelerometers, gyroscopes, and current sensors communicate through a simulated LoRa network to determine the health of each electricity pole.

The platform enables electricity board officers to monitor the electrical grid in real time, detect damaged or leaning poles, assign repair tasks to field technicians, and track maintenance progress through an interactive dashboard.

---

## Features

- Secure role-based login for Officers and Staff
- Officer dashboard displaying all poles with live health status
- Real-time monitoring of accelerometer, gyroscope, and current sensor data
- Pole health classification into Healthy, Warning, and Alert
- Individual pole details with embedded Google Maps location
- Repair task assignment with due dates
- Staff portal for viewing and updating assigned tasks
- Staff management (Add, Edit, Delete)
- Simulated LoRa gateway data including RSSI, SNR, and sensor payloads

---

## Technology Stack

**Backend**
- Python
- Flask

**Frontend**
- HTML5
- CSS3
- JavaScript

**Maps**
- Google Maps Embed API

**Communication**
- Simulated LoRa

**Database**
- In-memory Python Data Structures

---

## Project Structure

```text
overhead-conductor-fault-detection/

├── app.py
├── requirements.txt
├── README.md
├── static/
│   ├── css/
│   ├── js/
│   └── uploads/
└── templates/
    ├── index.html
    ├── dashboard.html
    ├── pole.html
    ├── person.html
    ├── staff.html
    ├── staffadd.html
    └── staffedit.html
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/Saadgipuniwala/overhead-conductor-fault-detection.git
```

Navigate to the project directory

```bash
cd overhead-conductor-fault-detection
```

Create a virtual environment

```bash
python -m venv venv
```

Activate the virtual environment

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
python app.py
```

Open your browser

```
http://localhost:5001
```

---

## Demo Credentials

### Officer

**Username:** saadgi

**Password:** officer123

### Staff Accounts

| Username | Password |
|----------|----------|
| komal | komal123 |
| mayurika | mayurika123 |
| shreya | shreya123 |
| sejal | sejal123 |
| navami | navami123 |

---

## My Contribution

As a member of **Team SYNKTRA**, I contributed to:

- Flask backend development
- Dashboard implementation
- User interface integration
- Task assignment workflow
- Testing and debugging
- Deployment and project integration

---

## Current Limitations

- Sensor readings are simulated.
- LoRa communication is simulated.
- Data is stored in memory and resets after every server restart.
- Passwords are stored in plain text for demonstration purposes.
- No automated testing has been implemented.

---

## Future Improvements

- SQLite or PostgreSQL database integration
- Secure password hashing
- Flask-Login authentication
- Real LoRa gateway integration
- MQTT communication support
- Email and SMS notifications
- REST API implementation
- Machine Learning-based fault prediction
- Advanced analytics dashboard
- CI/CD pipeline for cloud deployment

---

## Security Improvements

For production deployment, the following enhancements are recommended:

- Store the Flask Secret Key using environment variables.
- Secure and restrict the Google Maps API key.
- Hash passwords using Werkzeug Security.
- Replace in-memory data storage with a relational database.
- Implement proper authentication and authorization.

---

## Team

**Team SYNKTRA**

This project was developed as an IoT-enabled smart grid monitoring and fault detection solution for low-voltage electricity distribution systems.

---

## License

This project is intended for educational and demonstration purposes.
