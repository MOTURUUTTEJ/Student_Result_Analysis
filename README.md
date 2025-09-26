# Student_Result_Analysis

# Result Analysis System - A Dynamic Web Application

A modern, visually-rich, single-page web application designed for educational institutions to manage and analyze student results. This project leverages Firebase for real-time data management and features a sleek, animated user interface built with Tailwind CSS and `three.js`.

**(Recommended: Add a screenshot or GIF of the application in action here)**
`![Result Analysis System Screenshot](link_to_your_screenshot.png)`

---

## ✨ Features

* **Single-Page Application (SPA):** Seamless navigation between different sections without page reloads, powered by client-side routing using URL hashes.
* **Dual-Role Authentication:** A secure login system distinguishing between 'HOD' (Head of Department) and 'Staff' roles, with a separate registration flow.
* **Real-time Database:** Utilizes Google Firestore to ensure all data (student lists, subject reports, etc.) is updated in real-time across all connected clients.
* **Comprehensive Data Management:**
    * **Students:** Add new students and view a complete report of all students.
    * **Subjects:** Add new subjects (Theory, Practical, Lab) and view a consolidated report.
    * **Users:** Add new system users with different roles.
    * **Marks:** Input marks for specific students and subjects.
* **Dynamic Reporting:** All reports (Students, Subjects, Users, Marks) are dynamically generated and updated live from the database.
* **Stunning User Interface & Animations:**
    * **Animated Login Page:** Features a beautiful animated gradient background, floating 3D illustrations, and glassmorphism effects on the login form.
    * **Interactive Dashboard:** An immersive dashboard with a `three.js` powered animated 3D starfield background that reacts to mouse movement.
    * **Modern Aesthetics:** Styled with Tailwind CSS for a clean, responsive, and modern look.
    * **Micro-interactions:** Includes subtle hover effects, glowing animated buttons, and smooth page transitions for an enhanced user experience.

---

## 🛠️ Tech Stack

* **Frontend:** HTML5, JavaScript (ES6 Modules)
* **Styling:** Tailwind CSS
* **Backend & Database:** Google Firebase
    * **Firestore:** Real-time NoSQL database for storing all application data.
    * **Firebase Authentication:** Used to secure access to the Firestore database.
* **3D Graphics:** `three.js` for the animated dashboard background.

---

## 🚀 Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

You need a Google account to set up a Firebase project.

### Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
    ```

2.  **Set up Firebase:**
    * Go to the [Firebase Console](https://console.firebase.google.com/).
    * Click on "Add project" and create a new project.
    * Once the project is created, click on the "Web" icon (`</>`) to add a web app to your project.
    * Register the app and Firebase will provide you with a `firebaseConfig` object. Copy this object.
    * Go to the "Build" section in the left-hand menu and select **Firestore Database**. Click "Create database" and start in **test mode** for easy setup.

3.  **Configure the Application:**
    * Open the `HI.HTML` file.
    * Find the `firebaseConfig` constant within the `<script>` tag (around line 436).
    * Replace the placeholder values with the configuration object you copied from your Firebase project.
    ```javascript
    const firebaseConfig = {
        apiKey: "YOUR_API_KEY",
        authDomain: "YOUR_PROJECT.firebaseapp.com",
        projectId: "YOUR_PROJECT_ID",
        storageBucket: "YOUR_PROJECT.appspot.com",
        messagingSenderId: "YOUR_SENDER_ID",
        appId: "YOUR_APP_ID"
    };
    ```

4.  **Run the Application:**
    * Simply open the `HI.HTML` file in your web browser. No web server or build process is needed.

---

## Login Credentials

The application is pre-populated with two demo user accounts stored in local storage:

* **Role:** HOD
    * **Username:** `hod`
    * **Password:** `hod123`
* **Role:** Staff
    * **Username:** `staff`
    * **Password:** `staff123`

You can also create new accounts using the "Create one" link on the login page.
