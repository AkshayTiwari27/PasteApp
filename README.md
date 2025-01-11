---

# Paste App

A feature-rich pastebin clone built with React, Vite, and Tailwind CSS. The Paste App allows users to create, share, and manage text snippets effortlessly. With real-time updates, syntax highlighting, and a user-friendly interface, it's perfect for developers and anyone needing a reliable paste service.

## Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Scripts](#scripts)
- [Packages Used](#packages-used)
- [Project Structure](#project-structure)
- [Tailwind CSS Configuration](#tailwind-css-configuration)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- **Real-Time Updates**: Instantaneously see changes without refreshing the page.
- **Private and Public Pastes**: Control the visibility of your snippets.
- **Search Functionality**: Easily find pastes by keywords or tags.
- **Responsive Design**: Optimized for both desktop and mobile devices.

---

## Demo

Check out the live demo [here](https://paste-app-kk3m.vercel.app/pastes).
---

## Installation

### Prerequisites

- **Node.js**: Ensure you have Node.js installed. You can download it from [here](https://nodejs.org/).
- **npm**: Node Package Manager comes with Node.js. Alternatively, you can use `yarn`.

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/paste-app.git
```

### Step 2: Navigate to the Project Directory

```bash
cd paste-app
```

### Step 3: Install Dependencies

```bash
npm install
```

### Step 4: Configure Environment Variables

Create a `.env` file in the root directory and add the necessary environment variables:

```env
VITE_API_URL=https://api.pasteapp.example.com
VITE_AUTH_KEY=your-auth-key
```

> **Note**: Replace the placeholder values with your actual configuration.

### Step 5: Run the Development Server

```bash
npm run dev
```

Open your browser and navigate to `http://localhost:5173` to see the app in action.

---

## Usage

Once the development server is running:

1. **Create a Paste**:
   - Click on the "New Paste" button.
   - Enter your text snippet.
   - Choose the language for syntax highlighting (optional).
   - Set the paste visibility (public or private).
   - Save the paste to generate a unique URL.
2. **Manage Pastes**:
   - View your pastes in the dashboard.
   - Edit or delete pastes as needed.
3. **Search Pastes**:
   - Use the search bar to find pastes by keywords or tags.

---

## Scripts

- **`npm run dev`**: Starts the Vite development server with Hot Module Replacement (HMR).
- **`npm run build`**: Builds the application for production.
- **`npm run preview`**: Serves the production build locally for preview.
- **`npm run lint`**: Runs ESLint to analyze code for potential errors and enforce coding standards.
- **`npm run format`**: Formats the codebase using Prettier.

---

## Packages Used

### Dependencies

- **React**: JavaScript library for building user interfaces.
- **Vite**: Fast build tool and development server.
- **Tailwind CSS**: Utility-first CSS framework for rapid UI development.
- **Redux Toolkit**: Simplifies Redux state management.
- **React Router DOM**: Declarative routing for React applications.
- **React Hot Toast**: Elegant notifications for React.
- **Axios**: Promise-based HTTP client for API requests.
- **Prism.js**: Lightweight syntax highlighting library.

### Dev Dependencies

- **@vitejs/plugin-react**: Official Vite plugin for React, enabling Fast Refresh.
- **eslint**: Linter for identifying and fixing problems in JavaScript code.
- **eslint-plugin-react**: React specific linting rules for ESLint.
- **eslint-plugin-react-hooks**: Linting rules for React Hooks.
- **postcss**: Tool for transforming CSS with JavaScript plugins.
- **autoprefixer**: PostCSS plugin to parse CSS and add vendor prefixes.
- **prettier**: Code formatter.
- **eslint-config-prettier**: Disables ESLint rules that might conflict with Prettier.
- **eslint-plugin-prettier**: Runs Prettier as an ESLint rule.
- **typescript**: Superset of JavaScript adding static typing (if using TypeScript).

---

## Project Structure

```
paste-app/
│
├── node_modules/
├── public/
│   └── favicon.ico
├── src/
│   ├── assets/
│   │   └── logo.svg
│   ├── components/
│   │   ├── Header.jsx
│   │   ├── Footer.jsx
│   │   ├── PasteForm.jsx
│   │   └── PasteList.jsx
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── Login.jsx
│   │   ├── Register.jsx
│   │   └── Dashboard.jsx
│   ├── store/
│   │   └── index.js
│   ├── App.jsx
│   ├── main.jsx
│   ├── index.css
│   └── routes.jsx
│
├── .eslintrc.js
├── .prettierrc
├── tailwind.config.js
├── postcss.config.js
├── vite.config.js
├── package.json
├── README.md
└── .gitignore
```

---

## Tailwind CSS Configuration

The `tailwind.config.js` file is set up to scan all relevant files for Tailwind CSS classes and allows for theme customization and plugin integration.

```javascript
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    './index.html',
    './src/**/*.{js,ts,jsx,tsx}',
  ],
  theme: {
    extend: {
      colors: {
        primary: '#1D4ED8',
        secondary: '#9333EA',
      },
      fontFamily: {
        sans: ['Inter', 'sans-serif'],
      },
    },
  },
  plugins: [
    require('@tailwindcss/forms'),
    require('@tailwindcss/typography'),
  ],
}
```

### Steps to Customize Tailwind

1. **Extending the Theme**: Modify the `extend` section to add custom colors, fonts, spacing, etc.
2. **Adding Plugins**: Integrate Tailwind CSS plugins to enhance functionality, such as forms and typography.
3. **Purging Unused Styles**: Ensure that Tailwind purges unused styles in production for optimal performance.

---

## Contributing

Contributions are welcome! Follow these steps to contribute:

1. **Fork the Repository**: Click the "Fork" button on the repository page.
2. **Clone Your Fork**:

   ```bash
   git clone https://github.com/yourusername/paste-app.git
   ```

3. **Create a New Branch**:

   ```bash
   git checkout -b feature/your-feature-name
   ```

4. **Make Your Changes**: Implement your feature or fix.
5. **Commit Your Changes**:

   ```bash
   git commit -m "Add feature: your feature description"
   ```

6. **Push to Your Fork**:

   ```bash
   git push origin feature/your-feature-name
   ```

7. **Create a Pull Request**: Navigate to the original repository and submit a pull request.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgements

- [Vite](https://vitejs.dev/) - Next Generation Frontend Tooling
- [React](https://reactjs.org/) - A JavaScript library for building user interfaces
- [Tailwind CSS](https://tailwindcss.com/) - A utility-first CSS framework
- [Redux Toolkit](https://redux-toolkit.js.org/) - The official, opinionated, batteries-included toolset for efficient Redux development
- [React Router](https://reactrouter.com/) - Declarative routing for React

---

## Contact

For any inquiries or support, please contact [youremail@example.com](mailto:tiwariakshay590@gmail.com).

---

© 2025 Paste App. All rights reserved.
