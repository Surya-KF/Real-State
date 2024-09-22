
# Real Estate Web Application (MERN Stack)

## Overview

This project is a full-featured Real Estate web application built using the MERN stack (MongoDB, Express, React, and Node.js). The platform allows **buyers** and **sellers** to interact directly by sending messages to each other. Additionally, users can view **real-time property locations** on an integrated map.

## Key Features

- **User Authentication**: Secure login and registration for both sellers and buyers.
- **Property Listings**: Sellers can list properties with detailed information (photos, price, location, etc.).
- **Messaging System**: Buyers and sellers can exchange messages in real-time.
- **Real-Time Map**: Integrated with Google Maps API, allowing users to view property locations in real-time.
- **Responsive Design**: Fully optimized for desktop and mobile devices.
- **Admin Panel**: Admins can manage users, properties, and messages.

## Tech Stack

### Frontend:
- **React.js**: For building interactive user interfaces.
- **Redux**: For state management across the application.
- **React Router**: For navigation between different pages.
- **Socket.IO**: For real-time messaging between buyers and sellers.
- **Google Maps API**: To display real-time locations of properties.

### Backend:
- **Node.js**: For building the backend server.
- **Express.js**: For creating RESTful APIs.
- **MongoDB**: For storing user, property, and messaging data.
- **Mongoose**: As an ORM for MongoDB.
- **JWT**: For user authentication.
- **Socket.IO**: For real-time communication.

## Features Breakdown

1. **User Authentication**:
   - Users can sign up as a buyer or seller.
   - Secure login using JWT (JSON Web Tokens).

2. **Property Listings**:
   - Sellers can add, edit, and delete their property listings.
   - Buyers can browse and search properties by location, price, and type.

3. **Messaging System**:
   - Real-time chat between buyers and sellers using Socket.IO.
   - Notifications for new messages.
   
4. **Real-Time Location on Map**:
   - Sellers can set the exact location of their properties.
   - Buyers can view property locations in real-time on a Google Map embedded on the website.

5. **Admin Dashboard**:
   - Admins can manage all users, properties, and messages.
   - Ability to delete inappropriate content and handle user complaints.

## Installation and Setup

### Prerequisites:
- Node.js and npm
- MongoDB (local or cloud instance like MongoDB Atlas)
- Google Maps API Key

### Steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/real-estate-mern.git
   cd real-estate-mern
   ```

2. **Install Dependencies**:
   - For the backend (in the root folder):
     ```bash
     npm install
     ```
   - For the frontend (inside the `client` folder):
     ```bash
     cd client
     npm install
     ```

3. **Set Up Environment Variables**:
   Create a `.env` file in the root directory and add the following:
   ```
   MONGO_URI=<Your MongoDB connection string>
   JWT_SECRET=<Your secret key>
   GOOGLE_MAPS_API_KEY=<Your Google Maps API key>
   ```

4. **Run the Backend**:
   ```bash
   npm run server
   ```

5. **Run the Frontend**:
   Open another terminal, navigate to the `client` folder, and run:
   ```bash
   npm start
   ```
---

## Folder Structure

```
real-estate-mern/
├── client/                  # React frontend
├── models/                  # Mongoose models (User, Property, Message)
├── routes/                  # Express routes (auth, properties, messages)
├── controllers/             # Logic for handling requests (CRUD, messaging)
├── config/                  # MongoDB connection and environment setup
├── middleware/              # JWT authentication middleware
└── server.js                # Express server setup
```
---

## Future Enhancements

- Implement a rating and review system for properties.
- Add payment integration for secure transactions.
- Provide filters based on property type, budget, and amenities.
  
## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an Issue.

## License

This project is licensed under the MIT License.

---
