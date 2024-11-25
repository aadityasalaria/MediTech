# MediTech

MediTech is a web-based application designed to streamline doctor appointment bookings for users and enable health centers to manage their appointments efficiently. The project leverages modern technologies to deliver a seamless and interactive user experience.

---

## Features

- **User Portal**: Book and manage appointments with doctors.
- **Admin Portal**: Manage health center data and appointments.
- **Receptionist Portal**: Assist in booking and managing schedules for walk-in patients.
- **Role-Based Access Control**: Ensures data security and portal-specific operations.

---

## Technologies Used

### Backend

- **[Flask](https://flask.palletsprojects.com/en/2.0.x/)**: Lightweight Python framework for building web applications.
- **[MySQL](https://www.mysql.com/)**: Relational database for managing appointment and user data.
- **[Gunicorn](https://gunicorn.org/)**: Python WSGI HTTP Server to serve the Flask application.

### Frontend

- **HTML5**: For structuring the web pages.
- **CSS3**: For designing an intuitive and responsive user interface.
- **JavaScript**: Enhances interactivity and user experience.

### Deployment

- **Docker**: Containerization to simplify application deployment.
- **AWS EC2**: Cloud server for hosting the application.

---

## Project Structure

```plaintext
MediTech
├── Application
│   ├── Backend
│   │   ├── __init__.py
│   │   ├── views.py
│   ├── DBHandler
│   │   ├── __init__.py
│   │   ├── sqlhandler.py
│   ├── __init__.py
│   ├── create_app.py
├── static
│   ├── css
│   ├── js
├── templates
│   ├── *.html
├── Dockerfile
├── requirements.txt
├── main.py
└── README.md
```

---

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/<your-repo>/MediTech.git
cd MediTech
```

### 2. Create a Virtual Environment

```bash
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Setup MySQL Database

- Create a database named `meditech`.
- Update the database credentials in the configuration file (if needed).

### 5. Run the Application Locally

```bash
python main.py
```

Visit the application at [http://127.0.0.1:5000](http://127.0.0.1:5000).

---

## Deployment Guide

### Dockerized Deployment

1. Build the Docker image:

   ```bash
   docker build -t meditech-app .
   ```

2. Run the container:

   ```bash
   docker run -d -p 80:5000 meditech-app
   ```

### AWS Deployment

- Set up an EC2 instance.
- Copy the project files to the instance.
- Install Docker and run the container as described above.

---

## Future Enhancements

- Implement **email notifications** for appointment confirmations.
- Add **role management** for more granular access control.
- Expand **analytics dashboards** for health centers.

---

## Contributors

- **Aaditya Salaria**
- **Ritika Shinde**
- **Manvi Khurana**
- **Shreya Gakhar**

---