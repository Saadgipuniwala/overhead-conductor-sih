# overhead-conductor-fault-detection
Smart grid monitoring and fault detection system using Flask and simulated LoRa communication to monitor pole health, assign maintenance tasks, and visualize fault locations.

Developed by Team SYNKTRA.

Overview

Smart Voltage Breakage Detection System (LV_AC) is a Flask-based web application developed to monitor the health of low-voltage (LV) AC distribution poles using simulated IoT sensor data. Pole-mounted sensors such as accelerometers, gyroscopes, and current sensors communicate through a simulated LoRa network to determine the condition of each pole.

The application enables electricity board officers to monitor the grid in real time, identify damaged or leaning poles, assign repair tasks to field technicians, and track maintenance activities through an interactive web dashboard.

Features

• Secure role-based login for Officers and Staff

• Officer dashboard displaying all poles with their current health status

• Live monitoring of accelerometer, gyroscope, and current sensor readings

• Health classification into Healthy, Warning, and Alert states

• Pole details with embedded Google Maps location

• Task assignment for maintenance staff with due dates

• Staff portal to view assigned tasks and update task completion status

• Staff management including adding, editing, and deleting staff members

• Simulated LoRa gateway data including RSSI, SNR, and raw sensor payloads

Technology Stack

Backend
- Python
- Flask

Frontend
- HTML
- CSS
- JavaScript

Maps
- Google Maps Embed API

Communication
- Simulated LoRa

Database
- In-memory Python data structures

Project Structure

LV_AC/

├── app.py

├── requirements.txt

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

Installation

Clone the repository

```bash
git clone https://github.com/your-username/LV_AC.git
```

Navigate to the project directory

```bash
cd LV_AC
```

Create a virtual environment

```bash
python -m venv venv
```

Activate the environment

Windows

```bash
venv\Scripts\activate
```

Linux/macOS

```bash
source venv/bin/activate
```

Install the required packages

```bash
pip install -r requirements.txt
```

Run the application

```bash
python app.py
```

Open your browser and visit

```
http://localhost:5001
```

Live Demo

https://overhead-conductor-fault-detection-1.onrender.com

Demo Credentials

Officer

Username: saadgi

Password: officer123

Staff Accounts

Username: komal

Password: komal123

Username: mayurika

Password: mayurika123

Username: shreya

Password: shreya123

Username: sejal

Password: sejal123

Username: navami

Password: navami123

My Contribution

As a member of Team SYNKTRA, I contributed to:

- Flask backend development
- Dashboard implementation
- User interface integration
- Task assignment workflow
- Testing and debugging
- Deployment and project integration

Current Limitations

- Sensor readings are simulated.
- LoRa communication is simulated.
- Data is stored only in memory and resets after every restart.
- Passwords are stored in plain text for demonstration purposes.
- No automated testing has been implemented.

Future Improvements

- Integrate SQLite or PostgreSQL database
- Implement secure password hashing
- Add Flask-Login authentication
- Connect with real LoRa gateway devices
- MQTT integration
- Email and SMS notifications
- REST API support
- Machine Learning-based fault prediction
- Analytics dashboard
- Cloud deployment with CI/CD pipeline

Security Improvements

For production deployment, the following improvements are recommended:

- Store the Flask Secret Key using environment variables.
- Secure and restrict the Google Maps API key.
- Hash passwords using Werkzeug Security.
- Replace in-memory storage with a relational database.
- Implement proper authentication and authorization.

Team

Team SYNKTRA

This project was developed as an IoT-enabled smart grid monitoring and fault detection solution for low-voltage electricity distribution systems.

License

This project is intended for educational and demonstration purposes.
