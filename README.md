# HomelyHub App using MERN stack

Welcome to the MERN Stack Internship project repository, which contains the source code and materials for our MERN (MongoDB, Express, React, Node.js) stack internship program, is designed to replicate the core functionalities of the Airbnb platform.

## Table of Contents

- [About the Project](#about-the-project)
- [Architecture](#Architecture)
  - [Features](#Features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
- [Usage](#usage)

## About the Project

HomelyHub is a platform that lets people find and book unique places to stay while traveling. Whether it's a cozy home or a fancy villa, or room, you can experience a personalized stay. Hosts can also earn money by sharing their spaces. so, Explore the world with HomelyHub for a unique and comfy adventure!

## Architecture

The HomelyHub project using the MERN (MongoDB, Express.js, React, Node.js) stack is designed to replicate the core functionalities of the Airbnb platform. The architecture comprises a MongoDB database to store property and user data, while Express.js handles server-side logic and API endpoints. React is employed for building the user interface, providing a dynamic and responsive experience for property listings and bookings. Node.js serves as the runtime environment for server-side execution, ensuring seamless communication between the front and back ends. The project follows a modular structure, with components for user authentication, property search, and booking features. Redux is integrated for efficient state management, enabling a smooth flow of data within the application. Additionally, the project employs RESTful API principles to facilitate communication between the client and server, ensuring a scalable and maintainable codebase.

### Features:

- User Authentication: Allow users to sign up, log in, and manage their profiles i.e., update users profile and password.
- Search and Filters: Implement a search feature with filters to enable users to easily find properties based on location, dates, pricing, and amenities, enhancing the overall user experience.
- View Listings: Users can view detailed information about each accommodation, including photos, descriptions, amenities.
- Property Listings: Allow property owners to list their accommodations, providing details such as images, descriptions, amenities, and pricing, etc.
- Booking System: Develop a booking system that allows users to select desired dates, view pricing, and confirm reservations, with real-time updates on availability and booking status.
- User Profiles: Implement user profiles where individuals can manage their bookings, update personal information, and track their property listing activity
- Payment Integration: Integrate a secure payment gateway to handle transactions, allowing users to make reservations and property owners to receive payments seamlessly.
- Responsive Design: Ensure a responsive and visually appealing design that adapts to various devices, providing a consistent and user-friendly experience on both desktop and mobile platforms.

## Getting Started

To get started with this project, follow the instructions below.

### Prerequisites

- Node.js and npm installed
- MongoDB installed and running
- Git installed
- Stripe and Mailtrap configured for payment and email functionality, respectively.

### Installation

#### 1. Clone the Repository

To get started with this project, follow these steps:

- Open your terminal or command prompt.

- Clone the repository by running the following command.

```bash
git clone https://github.com/KalmathAjay/Mern-stack-internship
```

#### 2. Install Dependencies

- Navigate to the cloned directory and install the project dependencies.
- Backend dependencies:

```bash
cd HomelyHub/Backend
npm install
```

- Frontend dependencies:

```bash
cd HomelyHub/Frontend
npm install
```

### Configuration

#### Environment Variables

Update the .env file located in the backend configuration directory:

```bash
cd HomelyHub/Backend/config.env
```

and populate it with the following environment-specific variables:

```env
# Express Server Configuration
PORT=4000
NODE_ENV=DEVELOPMENT

# MongoDB Configuration
DB_LOCAL_URI=mongodb://127.0.0.1/HomelyHub

# JSON Web Token (JWT) Configuration
JWT_SECRET=
JWT_EXPIRES_TIME=90

# Frontend URL
FRONTEND_URL=http://localhost:3000

# Cloudinary Configuration (for image uploads)
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=

# MailTrap Configuration (for email functionality)
EMAIL_USERNAME=
EMAIL_PASSWORD=
EMAIL_HOST=
EMAIL_PORT=
EMAIL_FROM=

# Stripe Configuration (for payments)
STRIPE_SECRET_KEY=
STRIPE_API_KEY=
```

#### Database Setup

To set up the project's data, you can use a database file provided in this repository. Follow these steps to import the data into your MongoDB database:

- Import Data

You can import the data into your MongoDB database using the `mongoimport` command. Make sure you have MongoDB installed and running locally.

Run the following command, replacing `DB_NAME` with the name of your database and `data.json` with the correct path to the database file:

```bash
mongoimport --db DB_NAME --collection your_collection_name --file path/to/data.json --jsonArray
```

## Usage

#### 1. Starting the Backend

- Open a terminal.

- Navigate to the project's backend directory:

  ```bash
  cd path/to/backend
  npm start
  ```

#### 2. Starting the Frontend

- Open a second terminal.

- Navigate to the project's frontend directory:

  ```bash
  cd path/to/frontend
  npm start
  ```

---

For questions, reach out to kalmathajay@gmail.com
