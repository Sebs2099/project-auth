# PetCare Center

Welcome to PetCare Center! This web application provides a platform for users to register and log in, with potential features for managing pet-related information and inventory for a pet shop or care facility.

---

## Features

*   **User Authentication:**
    *   User registration (data stored in `public/database.json` for local development)
    *   User login
*   **Pet Management (Dashboard):**
    *   View a list of registered pets.
    *   Add new pets (name, type, age, image).
    *   Edit details of existing pets.
    *   Delete pets.
    *   (Note: Pet data is managed via API calls, likely to a local `json-server` using `public/database.json` during development).
*   **Landing Page:** Informative landing page for new users.

---

## Technologies Used

*   **Frontend:**
    *   HTML5
    *   CSS3
    *   Vanilla JavaScript (ES6+)
*   **Build Tool & Development Server:**
    *   Vite
*   **Libraries:**
    *   SweetAlert2 (for user notifications and alerts)

---

## Setup and Installation

To get a local copy up and running, follow these simple steps:

### Prerequisites

*   Node.js and npm (Node Package Manager) or yarn. You can download Node.js from [nodejs.org](https://nodejs.org/).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/project-auth.git 
    ```
    *(Replace `your-username/project-auth.git` with the actual repository URL if different)*
2.  **Navigate to the project directory:**
    ```bash
    cd project-auth
    ```
3.  **Install NPM packages:**
    ```bash
    npm install
    ```
    Or if you use yarn:
    ```bash
    yarn install
    ```

---

## Running the Project

After successfully installing the dependencies, you can run the project locally:

### Development Server

To start the development server (powered by Vite):

```bash
npm run dev
```
Or if you use yarn:
```bash
yarn dev
```
This will typically open the application in your default web browser at `http://localhost:5173`. If it doesn't open automatically, or if that port is busy, check the terminal output for the correct address.

### Production Build

To create a production-ready build:

```bash
npm run build
```
Or if you use yarn:
```bash
yarn build
```
This command will generate a `dist` folder containing the optimized static assets for your project. You can then preview this build locally using:
```bash
npm run preview
```
Or if you use yarn:
```bash
yarn preview
```

---

## Project Structure

The project follows a standard structure for web applications:

```
project-auth/
├── public/             # Static assets that are directly copied to the build output
│   └── database.json   # Likely a mock database for local development
├── src/                # Source files for the application
│   ├── css/            # CSS stylesheets
│   │   └── styles.css  # Main stylesheet
│   ├── js/             # JavaScript files
│   │   ├── dashboard.js # Logic for the user dashboard
│   │   ├── login.js     # Logic for the login page
│   │   ├── main.js      # Main JavaScript entry point, handles navigation
│   │   └── register.js  # Logic for the registration page
│   └── views/          # HTML view files
│       ├── dashboard.html
│       ├── login.html
│       └── register.html
├── .gitignore          # Specifies intentionally untracked files that Git should ignore
├── index.html          # Main entry HTML file (landing page)
├── package-lock.json   # Records exact versions of dependencies
├── package.json        # Project metadata, dependencies, and scripts
└── README.md           # This file
```

### Key Directories and Files:

*   **`index.html`**: The main landing page of the application.
*   **`src/`**: Contains all the source code.
    *   **`src/css/styles.css`**: Main stylesheet for the application.
    *   **`src/js/`**: Contains JavaScript modules.
        *   `main.js`: Handles initial navigation from the landing page.
        *   `login.js`, `register.js`, `dashboard.js`: Handle logic for their respective views.
    *   **`src/views/`**: HTML files for different pages/views of the application (login, register, dashboard).
*   **`public/`**: Static assets that are served as-is or copied to the build directory.
    *   `database.json`: Appears to be a JSON file used as a simple database, likely for storing user data or other application data locally during development.
*   **`package.json`**: Defines project dependencies, scripts (like `dev`, `build`), and metadata.
*   **`vite.config.js`** (if present, otherwise Vite uses defaults): Configuration file for Vite. *(Self-correction: I haven't seen this file yet, so I'll make a note that it might not exist and Vite might be using defaults)*

---

## Author

*   **Sebastian Cabarcas M.**
    *   GitHub: [@Sebs2099](https://github.com/Sebs2099) (Assuming this is the GitHub profile based on the organization meta tag. This should be verified.)

---

## Contributing

Contributions are welcome! Please follow these steps:

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## License

This project is licensed under the MIT License - see the `LICENSE.md` file for details (if one exists, otherwise specify the license).

*(Note: A `LICENSE.md` file is not currently present in the repository. It's good practice to add one.)*

---

## Acknowledgments

*   [Vite](https://vitejs.dev/) - Fast Frontend Tooling
*   [SweetAlert2](https://sweetalert2.github.io/) - Beautiful, responsive, customizable JavaScript alerts
*   Placeholder image from [Pixabay](https://pixabay.com/)

---
