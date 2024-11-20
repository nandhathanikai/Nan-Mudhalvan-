# Book a Doctor

## 📖 Project Overview  
**Book a Doctor** is a web application developed using the MERN stack (MongoDB, Express.js, React.js, and Node.js). The platform connects patients with doctors, enabling patients to book, reschedule, and cancel appointments while helping doctors manage their schedules efficiently. This project is designed to simplify the appointment booking process and provide a seamless user experience.

---

## 🚀 Features  

### For Patients:  
- **User Registration and Login**: Secure authentication using JWT.  
- **Search Doctors**: Search doctors by specialty, location, or availability.  
- **Book Appointments**: Easy booking with preferred dates and times.  
- **View Appointment History**: Track all past and upcoming appointments.  
- **Cancel/Reschedule Appointments**: Flexibility to manage appointments.  

### For Doctors:  
- **Profile Management**: Add personal and professional details.  
- **Appointment Management**: View, approve, or cancel appointments.  
- **Schedule Availability**: Define available time slots for appointments.  

---

## 🛠️ Tech Stack  

### Frontend:  
- **React.js**: UI development.  
- **React Router**: For navigation.  
- **Axios**: For API calls.  

### Backend:  
- **Node.js**: Server-side logic.  
- **Express.js**: Backend framework for routing and middleware.  

### Database:  
- **MongoDB**: NoSQL database for storing data.  

### Other Tools & Libraries:  
- **Multer**: For file uploads.  
- **Dotenv**: For environment variables.  
- **Cors**: To handle cross-origin requests.  
- **Bcrypt.js**: For password encryption.  
- **JSON Web Token (JWT)**: For secure authentication.  

---

---

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Project Structure](#project-structure)
5. [API Documentation](#api-documentation)
6. [Common Issues](#common-issues)
7. [Contributing](#contributing)
8. [License](#license)
9. [Contact](#contact)

---

## Prerequisites

Ensure the following software and tools are installed:

- **Node.js**: v16.x or later ([Download Here](https://nodejs.org/))
- **npm**: v8.x or later (comes with Node.js)
- **Git**: v2.0 or later ([Download Here](https://git-scm.com/))

---
## Installation

```bash
git clone https://github.com/srikanth230/Online-Complaint-Registration.git
cd code/backend
npm install
```

Customize the configuration file (`config.js`) to fit your environment (e.g., database settings).

---

## Usage

```bash
# Start the server
node index.js

# Optional: Run with live reload
npm install -g nodemon
nodemon index.js
```

The API runs on `http://localhost:3000` by default. Update the `config.js` file to change the port.

Use tools like Postman or `curl` to send requests and verify endpoints.

---

## Project Structure

```plaintext
code/
└── backend/
    ├── config.js          # Configuration settings for the application
    ├── index.js           # Main entry point for starting the application
    ├── node_modules/      # Directory for installed dependencies
    ├── package.json       # Lists dependencies and project metadata
    ├── .gitignore         # Specifies files to ignore in version control
    └── README.md          # Documentation file
```

---

## API Documentation

### Base URL

```
http://localhost:3000
```

### Endpoints

| Method | Endpoint            | Description                  |
|--------|---------------------|------------------------------|
| GET    | `/complaints`       | Fetch all complaints         |
| POST   | `/complaints`       | Create a new complaint       |
| PUT    | `/complaints/:id`   | Update an existing complaint |
| DELETE | `/complaints/:id`   | Delete a specific complaint  |

### Example Request (Create Complaint)

```json
POST /complaints
Content-Type: application/json
{
  "title": "Network Issue",
  "description": "Internet is not working in the office.",
  "status": "Open"
}
```

### Example Response

```json
{
  "id": 1,
  "title": "Network Issue",
  "description": "Internet is not working in the office.",
  "status": "Open",
  "created_at": "2024-11-18T12:34:56Z"
}
```

---

## Common Issues

### Error: Cannot find module
Ensure all dependencies are installed with:
```bash
npm install
```

### Port Conflict
Update the port number in `config.js` if another application is using the default port (3000).

### Database Connection Error
Verify the database credentials in `config.js`.

---

## Contributing

1. Fork the repository.
2. Create a new feature branch:
   ```bash
   git checkout -b feature/new-feature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push the branch:
   ```bash
   git push origin feature/new-feature
   ```
5. Submit a pull request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact

For questions or suggestions, reach out via GitHub  

