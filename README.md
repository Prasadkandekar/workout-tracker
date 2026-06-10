# Workout Tracker

A modern, responsive web application for tracking and managing your fitness workouts. Built with Vue.js, Tailwind CSS, and Supabase.

## 🎯 Features

- **User Authentication**: Secure login and registration system
- **Workout Management**: Create, view, and manage your workout routines
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Real-time Database**: Powered by Supabase for reliable data storage
- **Modern UI**: Built with Tailwind CSS for a clean, professional interface
- **Navigation**: Easy-to-use navigation system for seamless app navigation

## 🛠️ Tech Stack

- **Frontend Framework**: Vue.js 3
- **Styling**: Tailwind CSS
- **Backend/Database**: Supabase
- **Build Tool**: Webpack (via Vue CLI)
- **Linting**: ESLint
- **CSS Processing**: PostCSS
- **JavaScript Transpiler**: Babel

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v14 or higher)
- npm or yarn package manager
- A Supabase account

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/Prasadkandekar/workout-tracker.git
cd workout-tracker
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Environment Setup

Create a `.env` file in the project root and add your Supabase credentials:
```
VUE_APP_SUPABASE_URL=your_supabase_url
VUE_APP_SUPABASE_ANON_KEY=your_supabase_anon_key
```

### 4. Run Development Server
```bash
npm run serve
```

The application will be available at `http://localhost:8080`

### 5. Build for Production
```bash
npm run build
```

## 📁 Project Structure

```
workout-planner/
├── public/                 # Static assets
│   └── index.html         # Main HTML file
├── src/
│   ├── assets/            # CSS and image files
│   │   ├── tailwind.css   # Tailwind styles
│   │   └── images/        # Image assets
│   ├── components/        # Reusable Vue components
│   │   └── Navigation.vue # Navigation component
│   ├── views/             # Page components
│   │   ├── Create.vue     # Create workout page
│   │   ├── Home.vue       # Home/dashboard page
│   │   ├── Login.vue      # Login page
│   │   ├── Register.vue   # Registration page
│   │   └── ViewWorkout.vue # View workout details
│   ├── router/            # Vue Router configuration
│   │   └── index.js       # Route definitions
│   ├── store/             # Vuex/State management
│   │   └── index.js       # Store configuration
│   ├── supabase/          # Supabase configuration
│   │   └── init.js        # Supabase initialization
│   ├── App.vue            # Root component
│   └── main.js            # Application entry point
├── .eslintrc.js           # ESLint configuration
├── babel.config.js        # Babel configuration
├── postcss.config.js      # PostCSS configuration
├── tailwind.config.js     # Tailwind CSS configuration
├── package.json           # Project dependencies
├── .env                   # Environment variables (create this)
└── static.json            # Static hosting configuration
```

## 🔐 Authentication

The app includes user authentication with:
- **Register**: Create a new account
- **Login**: Sign in to your account
- **Logout**: Sign out and return to login

User data is securely stored in Supabase.

## 📝 Available Scripts

```bash
# Development
npm run serve              # Start development server

# Production
npm run build              # Build for production
npm run build:modern       # Build with modern JavaScript

# Linting
npm run lint               # Run ESLint
npm run lint --fix         # Fix ESLint issues

# Testing (if configured)
npm run test:unit          # Run unit tests
```

## 🎨 Styling

This project uses **Tailwind CSS** for styling. The configuration can be found in `tailwind.config.js`.

### Adding Custom Styles
Edit `src/assets/tailwind.css` for global styles.

## 🗄️ Database Schema (Supabase)

The application uses Supabase PostgreSQL database. Typical schema includes:
- **users**: User authentication and profile information
- **workouts**: Workout records with details
- **exercises**: Exercise definitions

## 🔄 State Management

State is managed using Vuex (or similar). Store configuration is in `src/store/index.js`.

## 🧭 Routing

Routes are configured in `src/router/index.js` with the following main pages:
- `/` - Home page
- `/login` - Login page
- `/register` - Registration page
- `/create` - Create new workout
- `/workout/:id` - View workout details

## 🌐 Deployment

### Deploy to Netlify/Vercel
1. Build the project: `npm run build`
2. Connect your GitHub repository
3. Set build command: `npm run build`
4. Set publish directory: `dist`

### Deploy to Heroku
The project includes `static.json` for static hosting configuration.

## 🐛 Troubleshooting

### Port Already in Use
```bash
npm run serve -- --port 3000
```

### Clear Node Modules
```bash
rm -r node_modules
npm install
```

### Environment Variables Not Loading
Restart your development server after updating `.env` file.

## 📚 Resources

- [Vue.js Documentation](https://vuejs.org)
- [Tailwind CSS Documentation](https://tailwindcss.com)
- [Supabase Documentation](https://supabase.com/docs)
- [Vue Router Guide](https://router.vuejs.org)

## 👤 Author

**Prasad Kandekar**
- GitHub: [@Prasadkandekar](https://github.com/Prasadkandekar)

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## ❓ Support

For support, please open an issue on the GitHub repository.

---

**Last Updated**: June 2026
