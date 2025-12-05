## 📖 About the Project

**ESPRIT Reclamation & Chatbot Interfaces** is a modern web application designed to streamline the process of submitting and managing complaints within Esprit University. It integrates a smart **Virtual Chatbot Assistant** to help students and staff navigate services efficiently.

Built with **HTML5** and **Tailwind CSS**, the project focuses on a responsive, user-friendly design that adheres to the university's visual identity.

---

## ✨ Key Features

### 🏛️ Core Functionality

- **User Dashboard**: A central hub to view status updates and recent activities.
- **Claim Management**:
  - **Submit Claims**: Intuitive forms for submitting new complaints (`new-claim-user.html`).
  - **Track History**: View the status and history of previous claims (`history.html`).
  - **Claim Details**: Deep dive into specific claim information (`details.html`).
- **Profile Management**: Update user details and preferences (`ProfileDetails.html`).

### 🤖 Intelligent Assistance

- **Virtual Chatbot**: An interactive assistant to answer queries in real-time (`ESPRITVirtualChatbotAssistant.html`).
- **Interaction History**: Review past conversations with the bot (`interactions.html`).
- **Feedback System**: Rate the chatbot's performance to improve future interactions (`ESPRITChatbotRatingPage.html`).

### 🔐 Security & Access

- **Secure Login**: Authentication gateway for students and admins (`Login.html`).

---

## 👥 Team Members

We are a team of dedicated developers working to improve the campus experience:

| Name                      | Role                 |
| ------------------------- | -------------------- |
| **Youssef Dhib**          | Full Stack Developer |
| **Aziz Logtari**          | Frontend Developer   |
| **Yassine Sayari**        | UI/UX Designer       |
| **Mohamed Habib Dhaoudi** | Backend Developer    |
| **Mohamed Ossema Meddeb** | Project Manager      |
| **Abderrahmen Jlassi**    | QA Engineer          |

---

## 🚀 Getting Started

Follow these steps to set up the project locally.

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari).
- **Node.js** & **npm** (Optional, only for recompiling Tailwind CSS).

### Installation

1.  **Clone the repository**:

    ```bash
    git clone https://github.com/your-username/esprit-interfaces.git
    cd esprit-interfaces
    ```

2.  **Install dependencies** (if you plan to edit CSS):
    ```bash
    npm install
    ```

### Running the Project

1.  **Simple Method**:

    - Navigate to the project folder.
    - Open `index.html` in your browser.
    - You will be redirected to the main application flow.

2.  **Development Mode** (for CSS updates):
    ```bash
    npm run build-css
    ```

---

## � Project Structure

```plaintext
reclamation-website/
├── 📁 assets/          # Images, icons, and static assets
├── 📁 css/             # Compiled CSS and Tailwind source
│   ├── main.css        # Final output file
│   └── tailwind.css    # Source file with directives
├── 📁 pages/           # Application views (HTML files)
│   ├── Dashboard.html
│   ├── Login.html
│   ├── list-complaints.html
│   └── ...
├── 📄 index.html       # Entry point (Redirects to app)
├── 📄 tailwind.config.js # Tailwind configuration
└── 📄 package.json     # Project metadata and scripts
```

---

## 🛠️ Technical Challenges & Solutions

During development, we encountered and solved several key technical challenges:

### 1. Mobile Responsive Sidebar

- **Problem**: The sidebar consumed too much screen real estate on mobile devices, breaking the layout.
- **Solution**: Implemented an off-canvas "hamburger" menu. The sidebar is hidden by default on mobile (`-translate-x-full`) and slides in smoothly when toggled, using a dark overlay to focus user attention.

### 2. Complex Form Layouts

- **Problem**: Aligning multiple input fields, text areas, and upload buttons (e.g., in the "New Claim" page) was inconsistent across devices.
- **Solution**: Leveraged **CSS Grid** (`grid-cols-1` to `md:grid-cols-3`) and **Flexbox** utilities from Tailwind. This allowed forms to automatically stack vertically on mobile while expanding to multi-column layouts on larger screens.

### 3. Visual Consistency

- **Problem**: Maintaining the strict Esprit brand identity (Red `#D2232A`, Font `Inter`) across all distinct pages.
- **Solution**: Defined custom colors in `tailwind.config.js` and applied global font settings. We used utility classes like `text-[#D2232A]` and `bg-[#D2232A]` to ensure exact color matching everywhere.

---

<div align="center">
  <sub>Built with ❤️ by the Esprit Integration Team</sub>
</div>
