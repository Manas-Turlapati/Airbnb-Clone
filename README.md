🏡 WanderLust — Airbnb Clone
A fully functional vacation rental web application built with the MERN-inspired stack (MongoDB, Express, Node.js) with server-side rendering using EJS. Users can browse, create, and manage property listings with image uploads, map integration, reviews, and secure authentication.

🚀 Live Demo

https://airbnbclone-manas.onrender.com


✨ Features

🔐 User Authentication — Register, Login, Logout with Passport.js (Local Strategy)
🏠 Listings CRUD — Create, Read, Update, Delete property listings
🖼️ Image Uploads — Cloud-based image storage via Cloudinary + Multer
🗺️ Map Integration — Interactive maps using Leaflet.js with GeoJSON coordinates
⭐ Reviews System — Add and delete reviews on listings
🛡️ Authorization — Only listing/review owners can edit or delete their content
💾 Session Management — Persistent sessions stored in MongoDB via connect-mongo
⚡ Flash Messages — Success and error notifications across the app
🔒 Security — HTTP-only cookies, method override, input validation with Joi


🛠️ Tech Stack
LayerTechnologyBackendNode.js, Express.jsDatabaseMongoDB, MongooseTemplatingEJS, EJS-MateAuthenticationPassport.js, passport-local-mongooseImage StorageCloudinary, MulterMapsLeaflet.jsSession Storeconnect-mongoValidationJoiDev ToolNodemon

📁 Project Structure
MajorProject/
├── controllers/
│   ├── listing.js       # Listing CRUD logic
│   ├── review.js        # Review logic
│   └── user.js          # Auth logic
├── models/
│   ├── listing.js       # Listing schema (with geo & image)
│   ├── review.js        # Review schema
│   └── user.js          # User schema
├── routes/
│   ├── listing.js       # /listings routes
│   ├── review.js        # /listings/:id/reviews routes
│   └── user.js          # /login, /register, /logout routes
├── views/               # EJS templates
├── public/              # Static assets (CSS, JS)
├── init/                # DB seed data
├── middleware.js         # Auth & validation middleware
├── cloudConfig.js       # Cloudinary configuration
└── app.js               # Entry point

⚙️ Getting Started
Prerequisites

Node.js v20.x
MongoDB Atlas account
Cloudinary account

Installation
bash# Clone the repository
git clone https://github.com/yourusername/MajorProject.git
cd MajorProject

# Install dependencies
npm install
Environment Variables
Create a .env file in the root directory:
envATLASDB_URL=your_mongodb_atlas_connection_string
SECRET=your_session_secret
CLOUD_NAME=your_cloudinary_cloud_name
CLOUD_API_KEY=your_cloudinary_api_key
CLOUD_API_SECRET=your_cloudinary_api_secret
Run the App
bash# Development
npm run dev

# Production
npm start
App runs on http://localhost:3000

🌱 Seed Database
bashnode init/index.js
<img width="1903" height="911" alt="image" src="https://github.com/user-attachments/assets/64ceb099-8fb6-412a-b429-840e1a666012" />
<img width="1914" height="902" alt="image" src="https://github.com/user-attachments/assets/5708bb8d-7f7a-4027-8bd0-236e80d0d300" />
<img width="1919" height="905" alt="image" src="https://github.com/user-attachments/assets/8c479154-d59c-4f0c-8a7a-ba153c06975e" />




🙌 Author
Built by Manas Turlapati
GitHub • LinkedIn
