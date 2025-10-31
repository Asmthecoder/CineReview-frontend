# Quick Start Guide

## Installation Steps

1. Open Command Prompt (cmd) or PowerShell in the `frontend-react` folder

2. Install dependencies:
   ```
   npm install
   ```

3. Start the development server:
   ```
   npm run dev
   ```

4. Open your browser to http://localhost:3000

## Demo Accounts

**Admin Account:**
- Username: admin
- Password: admin123

**Regular User:**
- Username: user  
- Password: user123

## What's Been Migrated

✅ All vanilla JavaScript converted to React components
✅ TMDB API integration with custom hooks
✅ Authentication system with React Context
✅ Movie browsing, search, and filtering
✅ Favorites and recently viewed (localStorage)
✅ Review system connected to backend
✅ Responsive design with Bootstrap 5
✅ Dark/light theme toggle
✅ All CSS styles migrated

## File Structure

- `/src/components/` - Reusable UI components
- `/src/pages/` - Page components (Home, Login, etc.)
- `/src/context/` - React Context providers (Auth, Theme)
- `/src/hooks/` - Custom React hooks
- `/src/utils/` - Helper functions and constants
- `/src/index.css` - Global styles (copied from original)

## Next Steps

1. Test all features in the browser
2. Compare with original vanilla JS version
3. Add any missing features
4. Deploy to production

## Backend API

The backend is already configured and should work without changes.
Make sure the server is running on Vercel or localhost.

## Troubleshooting

**Port already in use:**
Edit `vite.config.js` and change the port number

**API errors:**
Check that the backend server is running and CORS is enabled

**Module not found:**
Run `npm install` again

**Blank screen:**
Check browser console for errors
