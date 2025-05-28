# Timelock - Secure Password Manager

A password management application built with microservice architecture, developed as a learning project focusing on security, user control, and modern web development practices.

## Demo

Live Demo - See the project in action!  
🌐 **Deployed at:** [timelock.se](https://timelock.se)

https://github.com/user-attachments/assets/fb320d69-c714-4650-9060-f44906dc5846

## 📋 About the Project

This project was developed as part of the **1DV613 Software Development Project** course at Linnaeus University, during the first year of the Web Developer program. The project and documentation were developed over **10 weeks** as a learning exercise in modern web development.

### What does Timelock do?

Timelock is a password manager that aims to give users control over their passwords. The system includes:

- **Secure password storage** - Passwords are encrypted and stored safely
- **Password history tracking** - See when passwords were changed (without revealing old passwords)
- **Email verification** - Two-step authentication for added security
- **Microservice architecture** - Separate services for different functions
- **User privacy focus** - Built with privacy as a core principle

*Note: End-to-end encryption is part of the project vision and will be implemented in future updates.*

### Technologies I learned and used

- **Frontend:** EJS templates, HTML/CSS, JavaScript
- **Backend:** Node.js, Express.js
- **Database:** MongoDB with Mongoose
- **Security:** JWT tokens, cryptojs password hashing, CSRF protection
- **Tools:** Docker for containerization, Nginx, Google OAuth2
- **Testing:** Vitest for unit testing, manual testing

## 🏗️ Architecture

Timelock is built with three separate services:

- **Frontend-app:** Handles the user interface and web pages
- **Auth-service:** Manages user accounts and login
- **Password-service:** Stores and manages password data

## Architecture Diagram
![image](https://github.com/user-attachments/assets/b57b5ae1-65af-4e36-b396-ed2be13a829f)

## Installation

### What you need
- Node.js (version 14 or newer)
- MongoDB
- Docker (optional but recommended)

### Quick start with Docker
```bash
# Download the code
git clone https://github.com/BackEndByAlex/Timelock.git
cd Timelock

# Start everything with Docker
docker-compose up -d
```

### Manual setup
```bash
# Download the code
git clone https://github.com/BackEndByAlex/Timelock.git
cd Timelock

# Install packages for each part
cd frontend-app && npm install
cd ../auth-service && npm install  
cd ../password-service && npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your settings

# Start the application
npm run dev
```

## Current Features

- User registration and login
- Email verification with codes
- Google sign-in option
- Password storage with encryption
- Password change history (timestamps only)
- Automatic logout after being inactive
- Protection against common web attacks
- Works on mobile and desktop
- Basic password generation

## 🔒 Security Features I Implemented

- **JWT authentication** - Secure login tokens
- **Password hashing** - Passwords are never stored in plain text
- **Data encryption** - User data is encrypted in the database
- **Request protection** - CORS and CSRF security measures
- **Rate limiting** - Prevents spam and brute force attacks
- **Input checking** - Validates all user input
- **Session timeouts** - Automatic logout for security

## Testing

```bash
# Run all tests
npm test:unit

# Test individual services
cd auth-service && npm test:unit
cd password-service && npm test:unit
```

## What I Learned

Building Timelock taught me:

- **How to structure large applications** with multiple services
- **Web security basics** and how to protect user data
- **Authentication systems** and session management
- **Using Docker** to manage development environments
- **API design** and how services communicate
- **Writing tests** to ensure code works correctly
- **Deployment processes** and CI/CD basics
- **Project planning** and working with iterations

### Development Practices I Used
- ESLint for code quality
- Prettier for consistent formatting
- Consistent naming conventions
- Git for version control with meaningful commits

## 📚 Documentation

Detailed project documentation is available in the project wiki, including:

- Gitlab: [project wiki](https://gitlab.lnu.se/1dv613/student/aa227wr/project/-/wikis/home)
- Github: [project wiki](https://github.com/BackEndByAlex/frontend-app/wiki)

Project Planning & Analysis

Project Vision - Original vision and goals
Architecture & System Design - Technical architecture overview
Requirements Specification - Functional and non-functional requirements
Project Plan - Development timeline and methodology
Risk Analysis - Identified risks and mitigation strategies

Development Process

Sprint Backlogs - 8 iterations of development

Iteration 0-8: From initial design to final implementation


Testing Documentation - Test specifications and reports for each iteration

## Future Plans

The project will continue to evolve with planned features:

- **Complete end-to-end encryption** implementation
- Mobile app version
- Password sharing between users
- Browser extension
- Offline capability
- Improved password analysis
- Design improvements

## Project Status

- **Current version:** 1.0 (Course completion)
- **Development time:** 10 weeks (April-May 2025)
- **Status:** Core functionality complete, continuous improvements planned
- **Deployment:** Live at [timelock.se](https://timelock.se)

## 📝 License

This project is licensed under CC BY 4.0 - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Alexandru Antonescu**  
First-year Web Developer student at Linnaeus University
- GitHub: [@BackEndByAlex](https://github.com/BackEndByAlex)
- Student ID: aa227wr

##  Repository's

- [Frontend-service](https://github.com/BackEndByAlex/frontend-app)
- [Auth-service](https://github.com/BackEndByAlex/auth-service)
- [Password-service](https://github.com/BackEndByAlex/password-service)

---

*This project represents my learning journey in web development, showcasing practical application of security principles, microservice architecture, and modern development practices learned during my first year of studies.*
