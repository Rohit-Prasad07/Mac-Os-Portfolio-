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
