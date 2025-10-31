# CineReview - React Frontend

This is the React version of the CineReview movie review platform, built with Vite + React.

## 🚀 Features

- **Movie Discovery**: Browse popular, top-rated, upcoming, and now playing movies
- **Search Functionality**: Search for movies by title
- **User Authentication**: Login/Register with demo accounts
- **Favorites**: Add movies to your favorites list
- **Reviews**: Write and read movie reviews
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Dark/Light Theme**: Toggle between dark and light modes
- **Admin Panel**: Admin users can manage the platform

## 🛠️ Tech Stack

- **React 18** - UI library
- **Vite** - Build tool and dev server
- **React Router DOM** - Client-side routing
- **Bootstrap 5** - CSS framework
- **Font Awesome** - Icons
- **Chart.js** - Data visualization (for analytics)
- **TMDB API** - Movie data
- **Custom Backend API** - User reviews

## 📦 Installation

1. **Install dependencies:**
   ```bash
   cd frontend-react
   npm install
   ```

2. **Start the development server:**
   ```bash
   npm run dev
   ```

3. **Open your browser:**
   Navigate to `http://localhost:3000`

## 🏗️ Build for Production

```bash
npm run build
```

The optimized build will be in the `dist` folder.

## 🧪 Demo Accounts

- **Admin**: 
  - Username: `admin`
  - Password: `admin123`

- **Regular User**:
  - Username: `user`
  - Password: `user123`

## 📁 Project Structure

```
frontend-react/
├── public/              # Static assets
├── src/
│   ├── components/      # Reusable React components
│   │   ├── Navbar.jsx
│   │   ├── Footer.jsx
│   │   ├── Hero.jsx
│   │   ├── MovieCard.jsx
│   │   ├── FilterButtons.jsx
│   │   ├── Pagination.jsx
│   │   └── ScrollToTop.jsx
│   ├── pages/           # Page components
│   │   ├── Home.jsx
│   │   ├── Login.jsx
│   │   ├── Register.jsx
│   │   ├── MovieDetails.jsx
│   │   ├── Dashboard.jsx
│   │   └── Admin.jsx
│   ├── context/         # React Context providers
│   │   ├── AuthContext.jsx
│   │   └── ThemeContext.jsx
│   ├── hooks/           # Custom React hooks
│   │   ├── useMovies.js
│   │   ├── useReviews.js
│   │   └── useLocalStorage.js
│   ├── utils/           # Utility functions
│   │   ├── constants.js
│   │   └── helpers.js
│   ├── assets/          # Images, fonts, etc.
│   ├── App.jsx          # Main app component
│   ├── main.jsx         # Entry point
│   └── index.css        # Global styles
├── index.html           # HTML template
├── package.json         # Dependencies and scripts
└── vite.config.js       # Vite configuration
```

## 🔑 Key Features Explained

### Authentication
- Uses React Context API for global auth state
- Demo accounts stored in localStorage
- Protected routes (Dashboard, Admin panel)

### Movie Data
- Fetches from TMDB API
- Custom hooks (`useMovies`, `useMovieDetails`) for data fetching
- Search, filter, and pagination support

### Reviews
- Connects to custom backend API
- CRUD operations for reviews
- Rating system (1-5 stars)

### Favorites & History
- Stored in localStorage
- User-specific data
- Persists across sessions

### Styling
- Dark/light theme support
- Bootstrap 5 for responsive layout
- Custom CSS with CSS variables
- Smooth animations and transitions

## 🌐 API Endpoints

### TMDB API
- Popular: `/movie/popular`
- Top Rated: `/movie/top_rated`
- Upcoming: `/movie/upcoming`
- Now Playing: `/movie/now_playing`
- Search: `/search/movie`
- Details: `/movie/{id}`

### Backend API
- Get Reviews: `GET /api/v1/reviews/movie/{movieId}`
- Add Review: `POST /api/v1/reviews/new`
- Update Review: `PUT /api/v1/reviews/{reviewId}`
- Delete Review: `DELETE /api/v1/reviews/{reviewId}`

## 🎨 Customization

### Change Theme Colors
Edit CSS variables in `src/index.css`:
```css
:root {
  --primary-gradient: linear-gradient(145deg, #d4a574 0%, #8b6f47 100%);
  --bg-primary: #0d0d0d;
  --text-primary: #e8d5b7;
  /* ... */
}
```

### Add New Features
1. Create component in `src/components/`
2. Add route in `src/App.jsx`
3. Create custom hook if needed in `src/hooks/`

## 📝 Notes

- This is a demo project using localStorage for authentication
- In production, implement proper backend authentication (JWT, OAuth, etc.)
- TMDB API key is included for demo purposes
- Backend API is deployed on Vercel

## 🤝 Contributing

Feel free to submit issues and pull requests!

## 📄 License

MIT License

---

Built with ❤️ using React + Vite
