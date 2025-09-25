# TerraTrack

TerraTrack is a full-stack travel platform for discovering, listing, and reviewing unique travel destinations. Users can browse curated listings, filter by categories, search destinations, add new listings, and leave reviews.

## Features

- User authentication (signup, login, logout)
- Browse all travel listings with images, price, and location
- Filter listings by category (e.g., Beach, Mountain, City, etc.)
- Search listings by title, location, or country
- Add new listings with image upload (Cloudinary integration)
- Edit and delete your own listings
- Leave reviews and ratings on listings
- Responsive UI with Bootstrap 5 and custom CSS
- Flash messages for user feedback
- MongoDB for data storage

## Tech Stack

- Node.js, Express.js
- MongoDB, Mongoose
- Passport.js (authentication)
- EJS templating with EJS-Mate layouts
- Bootstrap 5, FontAwesome, Google Fonts
- Multer & Cloudinary for image uploads
- Joi for input validation
- connect-mongo for session storage

## Getting Started

### Prerequisites

- Node.js (v14+ recommended)
- MongoDB (local or Atlas)
- Cloudinary account (for image uploads)

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/terratrack.git
   cd terratrack
   ```

2. **Install dependencies:**
   ```sh
   npm install
   ```

3. **Set up environment variables:**

   Create a `.env` file in the root directory with the following:

   ```
   ATLAS_DB_URL=your_mongodb_connection_string
   SECRET=your_session_secret
   CLOUD_NAME=your_cloudinary_cloud_name
   CLOUD_API_KEY=your_cloudinary_api_key
   CLOUD_API_SECRET=your_cloudinary_api_secret
   ```

4. **Seed the database (optional):**

   - To seed categories:
     ```sh
     node init/categorydata.js
     ```
   - To seed sample listings:
     ```sh
     node init/data.js
     ```

5. **Start the server:**
   ```sh
   node app.js
   ```
   The app will run on [http://localhost:8080](http://localhost:8080).

## Project Structure

- `app.js` – Main Express app
- `models/` – Mongoose models (User, Listing, Review, Category)
- `controllers/` – Route controllers
- `routes/` – Express route definitions
- `views/` – EJS templates
- `public/` – Static assets (CSS, JS, images)
- `utils/` – Utility modules (error handling, async wrapper)
- `init/` – Seed scripts for categories and listings

## Deployment

- Ready for deployment on Vercel (see `vercel.json`)
- Configure environment variables in your deployment platform

## License

[MIT](LICENSE)

---

**Developed by Saumya Raj**
- **Linkedin** [Saumya Raj](https://www.linkedin.com/in/saumyaraj128/)
- **Github** [SaumyaRaj128](https://github.com/SaumyaRaj128)
