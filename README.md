# ReactP - Desktop-Like UI Application

A modern React application featuring a macOS-inspired desktop interface with draggable, resizable windows, a dock, and navigation components. Built with React 19, Vite, and Sass.

## 🎨 Features

- **Draggable & Resizable Windows** - Interactive window management using `react-rnd`
- **Dock Navigation** - Quick access dock similar to macOS
- **Navigation Bar** - Customizable navigation header
- **DateTime Display** - Real-time date and time information
- **Responsive Design** - Built with SCSS for flexible styling
- **Fast Refresh** - Instant HMR during development with Vite

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ReactP.git
cd ReactP
```

2. Install dependencies:
```bash
npm install
```

### Development

Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5173`

### Build

Create a production build:
```bash
npm run build
```

### Preview

Preview the production build locally:
```bash
npm run preview
```

### Linting

Check code quality:
```bash
npm run lint
```

## 📁 Project Structure

```
src/
├── App.jsx                 # Main application component
├── app.scss               # Application styles
├── main.jsx               # Entry point
├── components/
│   ├── DateTime.jsx       # Date/time display component
│   ├── Dock.jsx           # Dock navigation component
│   ├── dock.scss          # Dock styling
│   ├── Nav.jsx            # Navigation bar component
│   ├── nav.scss           # Navigation styling
│   └── windows/
│       ├── MacWindow.jsx  # Window component
│       └── window.scss    # Window styling
└── assets/                # Static assets

public/
├── doc-icons/             # Document icons
└── navbar-icons/          # Navigation bar icons
```

## 🛠️ Technologies

- **React 19** - UI framework
- **Vite** - Build tool and dev server
- **Sass** - CSS preprocessor
- **react-rnd** - Draggable and resizable components
- **ESLint** - Code quality tool

## 📦 Dependencies

- `react@^19.2.0` - Core React library
- `react-dom@^19.2.0` - React DOM rendering
- `react-rnd@^10.5.2` - Drag and resize functionality
- `sass@^1.97.3` - Sass compiler

## 🎯 Usage

The main App component manages the layout and renders the navigation bar, dock, and window components. Windows are draggable and resizable using react-rnd, providing a desktop-like experience.

### Adding New Windows

Create new window components in `src/components/windows/` and import them in your main App component.

### Customizing Styles

Modify SCSS files in their respective component directories to customize the appearance.

## 📝 License

This project is open source and available under the MIT License.

## 👤 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact

For questions or suggestions, please open an issue on GitHub.

---

## 🎤 Interview Q&A

To help you discuss this project during interviews, below are common questions along with sample answers that highlight the architecture, technologies, and development decisions.

### ❓ What is the purpose of this project?
**Answer:** This is a React application that simulates a macOS‑like desktop environment in the browser. It allows users to open, drag, resize, and interact with windows, mimicking desktop window management. The goal was to practice advanced component architecture, manage state across multiple draggable elements, and explore UI/UX concepts using React and modern tooling.

### ❓ Which technologies did you choose and why?
**Answer:** I used React 19 for its component model and hooks API. Vite provides a fast development server with hot module replacement, making iterative UI work efficient. Sass was chosen for modular and nested styling, keeping CSS maintainable. For drag/resize functionality, `react-rnd` is a lightweight library that integrates well with React. ESLint ensures consistent code quality.

### ❓ How is the project structured?
**Answer:** The `src` directory contains the main entry points and the `components` folder. Each component has its JSX and associated SCSS file. Windows live under `components/windows/` so adding new window types is straightforward. This separation promotes reusability and easier style overrides.

### ❓ How did you manage state for draggable windows?
**Answer:** State management lives in the main `App.jsx` which tracks open windows and their properties. Each window component receives props for position, size, and callbacks to update state when dragged or resized. This keeps the source of truth centralized while allowing individual windows to handle interaction details.

### ❓ How would you scale this application?
**Answer:** For larger apps, I'd introduce a state management library like Redux or Zustand to handle complex interactions. Dynamic window content could be lazy‑loaded using React's `lazy` and `Suspense`. The styling could be migrated to CSS modules or utility frameworks if needed. I’d also add accessibility features and keyboard support for window navigation.

### ❓ What were some challenges you faced?
**Answer:** Coordinating multiple draggable/resizable components proved tricky, especially ensuring performance when many windows are present. I solved it by memoizing components and minimizing re‑renders using `React.memo`. Another challenge was designing the dock and nav to reflect state changes; I used props and event handlers to keep them in sync.

### ❓ How do you test or lint the project?
**Answer:** The project uses ESLint (configured in `eslint.config.js`) for code linting, run via `npm run lint`. For unit or integration tests, you could integrate Jest or React Testing Library; those aren't included yet but can be added as needed.

---

Feel free to tailor these answers with your personal experience and any additional features you build upon this foundation.

