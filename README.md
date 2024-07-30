# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

# Guide to run these projects:
1.Create Your Vite Project:
```bash
npm create vite@latest my-project -- --template react
cd my-project
```
2.Install Tailwind CSS
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```
3.Configure Template Paths:
Edit tailwind.config.js.
```bash
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
4.Add Tailwind Directives:
Update ./src/index.css:
```bash
@tailwind base;
@tailwind components;
@tailwind utilities;
```
5.Start your build process
```bash
npm run dev
```
6.Your Page is displayed.
