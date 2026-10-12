# 𝕏 Twitter Clone — HTML & Tailwind CSS

A responsive frontend clone of the Twitter/X user interface, built using **HTML5 and Tailwind CSS**. This project recreates the familiar dark-themed X layout, including the navigation sidebar, post composer, timeline area, and discovery sidebar.

Built as a hands-on frontend development project to practice responsive layouts, utility-first CSS, and modern web UI design.

## 📸 Preview
![X Twitter Clone - Social Website](images/Preview.png)

## ✨ Features

- **Dark Theme:** Black background with white text and subtle borders.
- **Responsive Layout:** Adapts the three-column interface to different screen sizes.
- **Navigation Sidebar:** Home, Explore, Notifications, and other navigation items.
- **Post Composer:** An input area for drafting a post.
- **Discovery Sidebar:** Search, trending topics, and suggested accounts.
- **Material Symbols:** Icons for navigation and interface elements.
- **Tailwind CSS:** Utility classes for layout, spacing, typography, and responsiveness.
- **Vite Development Server:** Local development server for previewing the project.

> **Note:** This is a frontend UI clone, not a complete social networking application. Features such as real authentication, database storage, and publishing posts to a server are not included unless separately implemented.

## 🛠️ Technologies Used

- HTML5
- Tailwind CSS 3.4.19
- JavaScript (where applicable)
- Node.js and npm
- Vite
- Google Material Symbols


**File descriptions:**

- `index.html` — Contains the webpage structure and Tailwind CSS classes.
- `css/input.css` — Contains the Tailwind CSS directives.
- `css/output.css` — Contains the generated stylesheet used by the webpage.
- `images/favicon.ico` — The browser tab icon.
- `package.json` — Contains project metadata, dependencies, and npm scripts.
- `package-lock.json` — Records the resolved npm dependency versions.
- `tailwind.config.js` — Configures which files Tailwind scans for CSS classes.
- `.gitignore` — Specifies files and folders Git should ignore.

Your actual repository may contain additional files or folders.

## ⚙️ Prerequisites

Before running this project, install:

1. **Node.js and npm:** Download them from [nodejs.org](https://nodejs.org/).
2. **Git:** Download it from [git-scm.com](https://git-scm.com/).
3. **A code editor:** Visual Studio Code is recommended.
4. **A modern web browser:** Chrome, Edge, Firefox, or another compatible browser.

Verify your installations by opening a terminal and running:

```bash
node -v
npm -v
git --version
```

If these commands display version numbers, the required tools are available.

## 🚀 Getting Started

Follow these steps to download and run the project on your computer.

### Step 1: Clone the repository

Open your terminal or VS Code terminal and run:

```bash
git clone https://github.com/YOUR-USERNAME/twitter-clone-tailwindcss.git
```

Replace `YOUR-USERNAME` with your GitHub username.

Alternatively, open the repository on GitHub, select **Code → Download ZIP**, and extract the ZIP file.

### Step 2: Open the project folder

Navigate into the project directory:

```bash
cd twitter-clone-tailwindcss
```

If you downloaded the ZIP file, open the extracted folder in Visual Studio Code.

### Step 3: Install dependencies

Run the following command from the project root:

```bash
npm install
```

This installs the dependencies listed in `package.json`, including Tailwind CSS and Vite.

### Step 4: Generate the Tailwind CSS file

Run:

```bash
npm run build
```

The configured build script generates `css/output.css` from `css/input.css` and watches for changes.

**Important:** Because the script uses `--watch`, keep this terminal open while developing. If the command reports a missing input file or configuration error, check your folder paths and Tailwind configuration.

### Step 5: Start the development server

Open a **second terminal** in the same project directory and run:

```bash
npm run dev
```

Vite will display a local URL in the terminal, usually similar to:

```text
http://localhost:5173/
```

Open the exact URL printed by Vite in your browser to view the clone.

Keep both terminals running while you work: one for Tailwind CSS compilation and one for the Vite development server.

## 🎨 How Tailwind CSS Works in This Project

Tailwind CSS lets you style HTML elements using utility classes.

For example:

```html
<body class="bg-black text-white overflow-x-hidden">
```

This applies a black background, white text, and horizontal overflow control.

The `input.css` file contains:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Tailwind scans the files specified in `tailwind.config.js` and generates the corresponding CSS rules in `output.css`.

If you add new Tailwind classes, make sure the files containing those classes are included in the Tailwind `content` configuration.

## 🧪 Troubleshooting

### 1. The page loads without styling

- Confirm that `css/output.css` exists.
- Check that `index.html` links to `./css/output.css`.
- Run `npm run build` and check the terminal for errors.
- Ensure the Tailwind `content` paths include `index.html`.

### 2. `npm install` fails

- Verify that Node.js and npm are installed.
- Check your internet connection.
- Read the error message in the terminal before trying again.

### 3. The Vite command is not recognized

Run:

```bash
npm install
npm run dev
```

Make sure you are inside the project folder containing `package.json`.

### 4. Icons are missing

The project uses Google Material Symbols. Check your internet connection and confirm that the font stylesheet is loaded in `index.html`.

### 5. Changes to Tailwind classes do not appear

Keep the Tailwind watch process running. Verify that the edited HTML file is covered by `tailwind.config.js`, then check that `output.css` is being regenerated.

## 📱 Responsive Design

The interface uses Tailwind CSS responsive utilities, such as `sm:`, `md:`, `lg:`, and `xl:`, to adjust element sizes and visibility at different viewport widths.

For example:

```html
<span class="hidden sm:inline">
  Home
</span>
```

This hides the Home label on smaller screens and displays it at the `sm` breakpoint and above.

## 📚 Learning Objectives

This project can help beginners practice:

- Structuring pages with HTML5.
- Understanding Tailwind CSS utility classes.
- Building layouts with Flexbox.
- Using responsive breakpoints.
- Working with icons and external font resources.
- Managing frontend dependencies with npm.
- Running a project with Vite.
- Using Git and GitHub to publish a portfolio project.

## 🔮 Future Improvements

Possible improvements include:

- Add functional navigation and interactive buttons.
- Implement a working post composer.
- Add JavaScript interactions.
- Connect a backend and database.
- Implement authentication.
- Add a theme switcher.
- Improve keyboard accessibility and mobile usability.
- Deploy the project using a static hosting service.

## 🤝 Contributing

Contributions, suggestions, and beginner-friendly improvements are welcome.

1. Fork this repository.
2. Create a new branch.
3. Make your changes.
4. Commit your changes.
5. Open a pull request.

## ⚠️ Disclaimer

This project is an educational, unofficial UI recreation inspired by Twitter/X. It is not affiliated with, endorsed by, or connected to X Corp. or Twitter. All respective trademarks and brand assets belong to their owners.

## 👨‍💻 Author

**Zain Ul Abidin**

GitHub: [@zain-dev-ai-ml](https://github.com/zain-dev-ai-ml)

If you find this project helpful for learning frontend development, consider giving the repository a ⭐ on GitHub!

---

Made with ❤️ using HTML and Tailwind CSS.
