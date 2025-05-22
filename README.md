

---

# 🏠 Airbnb Clone (Server-Side Rendered)

A fully functional Airbnb clone built using the **MERN stack (without React)**, following **MVC architecture**, and rendered via **EJS templates**. This project supports core Airbnb features like listing properties, leaving reviews, managing users, and viewing maps.

---

## 🔧 Tech Stack

- **MongoDB** – NoSQL database for storing users, listings, and reviews
- **Express.js** – Backend server framework
- **EJS** – Templating engine for server-side rendering
- **Bootstrap** – Frontend responsive design (optimized for Windows)
- **Multer** – File upload middleware for handling listing images
- **Cloudinary** – Cloud storage for uploaded images
- **Joi** – Input validation for user data and form submissions
- **Unique ID Generator Library** – Generates unique identifiers
- **Render** – Hosting platform for deployment
- **REST API** – Organized routing for backend functionality

---

## ✨ Features

- 🏡 **Listings** – Add, view, update, and delete property listings with images
- ⭐ **Reviews** – Authenticated users can leave and manage reviews
- 👤 **Users** – Signup, login, session handling, and authorization
- 🗺️ **Maps** – Location-based rendering of listings using map integration
- 📱 **Responsive (Windows only)** – Mobile responsiveness with Bootstrap (tuned for Windows environment)

---

## 🧱 Project Architecture

```

airbnb-clone/
│
├── models/            # Mongoose schemas for Listings, Reviews, Users
├── routes/            # Route handlers for listings, users, reviews
├── controllers/       # MVC controllers for logic separation
├── views/             # EJS templates (layouts, partials, pages)
├── public/            # Static assets (CSS, JS, images)
├── utils/             # Helper functions (e.g., unique ID generator)
├── middlewares/       # Custom middleware (e.g., validation, auth)
├── uploads/           # Temporary storage for multer
├── .env               # Environment variables
├── app.js             # Main Express app
└── package.json

````

---

## 🚀 Live Demo

🔗 [View Live on Render](https://air-bnb-project-uio3.onrender.com/listings)

---

## 📦 Installation (Local Development)

### Prerequisites

- Node.js and npm
- MongoDB (Local or Atlas)
- Cloudinary account
- Render (for hosting)

### Steps

1. **Clone the repo**

```bash
git clone https://github.com/yourusername/airbnb-clone.git
cd airbnb-clone
````

2. **Install dependencies**

```bash
npm install
```

3. **Set up `.env` file**

```env
PORT=3000
DB_URL=mongodb://localhost:27017/airbnb-clone
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
SESSION_SECRET=your_random_secret
```

4. **Run the server**

```bash
node app.js
```

Visit `http://localhost:3000` in your browser.

---

## 📁 Cloud & Image Upload

* **Multer** is used for handling file uploads on the server.
* **Cloudinary** is integrated to store and serve images from the cloud.
* Uploaded listing images are stored securely and accessed via URLs.

---

## ✅ Validation

All user inputs (sign-up, login, listings, reviews) are validated using **Joi** schemas to ensure clean and secure data handling.

---

## 🧪 API Overview

* **GET /** – Home page with listings
* **GET /listings/\:id** – Detailed listing page
* **POST /listings** – Create a new listing (image + data)
* **POST /reviews/\:listingId** – Add a review to a listing
* **POST /register /login /logout** – Auth routes for users

---

## 🛠️ Author & Credits

Built with ❤️ by **Gaurav Pawar**

🔗 [Portfolio](https://gauravpawar.netlify.app)

---

## 📌 Notes

* UI is fully responsive only for **Windows viewports**.
* Make sure to replace all placeholders like `yourusername`, `your_cloud_name`, etc., before running the project.

---

## 🏁 Future Improvements

* React-based frontend for more dynamic experience
* Admin dashboard for property management
* Enhanced mobile responsiveness
* Google Maps full API integration

