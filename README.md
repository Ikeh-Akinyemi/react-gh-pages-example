# React GitHub Pages Example

This repository demonstrates how to deploy a React application to GitHub Pages, set up proper routing with React Router, and implement automated deployment using GitHub Actions.

## Demo

You can see a live demo of this project at: https://Ikeh-Akinyemi.github.io/react-gh-pages-example/

## Features

- ✅ React 18 application created with Create React App
- ✅ GitHub Pages deployment configuration
- ✅ Client-side routing with React Router (HashRouter)
- ✅ Automated deployment with GitHub Actions
- ✅ Environment variables and secrets management

## Getting Started

### Prerequisites

- Node.js 18+ and npm
- Git

### Installation

1. Clone this repository:

```bash
git clone https://github.com/Ikeh-Akinyemi/react-gh-pages-example.git
cd react-gh-pages-example
```

2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm start
```

## Deployment

### Manual Deployment

To manually deploy the app to GitHub Pages:

```bash
npm run deploy
```

This will build the app and publish it to the `gh-pages` branch of your repository.

### Automated Deployment with GitHub Actions

This repository is set up to automatically deploy to GitHub Pages whenever changes are pushed to the main branch. The GitHub Actions workflow:

1. Checks out the code
2. Sets up Node.js
3. Installs dependencies
4. Builds the project
5. Deploys to GitHub Pages

## Environment Variables

To use environment variables:

1. Go to your GitHub repository settings
2. Navigate to Secrets and Variables > Actions
3. Add a new repository secret with the name `REACT_APP_API_KEY`
4. Set the value to your API key

The value will be accessible in your React app via `process.env.REACT_APP_API_KEY`.

## Common Issues

If you encounter any of these common issues:

- **Blank page after deployment**: Ensure your `homepage` in `package.json` matches your GitHub Pages URL.
- **404 errors on page refresh**: This project uses HashRouter to prevent this issue.
- **Missing assets**: Make sure all assets use relative paths or `process.env.PUBLIC_URL`.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.