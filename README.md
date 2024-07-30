# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

# Guide to run these projects:
1.Create your project
Start by creating a new Vite project if you don’t have one set up already. The most common approach is to use Create Vite.
```bash
npm create vite@latest my-project -- --template react
cd my-project
```
2.Install Tailwind CSS
Install tailwindcss and its peer dependencies, then generate your tailwind.config.js and postcss.config.js files.
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```
3.Configure your template paths
Add the paths to all of your template files in your tailwind.config.js file.
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
4.Add the Tailwind directives to your CSS
Add the @tailwind directives for each of Tailwind’s layers to your ./src/index.css file.
```bash
@tailwind base;
@tailwind components;
@tailwind utilities;
```
5.Start your build process
Run your build process with npm run dev.
```bash
npm run dev
```
6.Your Page is displayed.
