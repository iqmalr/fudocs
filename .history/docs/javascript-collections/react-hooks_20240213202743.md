---
sidebar_position: 1
---

<!-- # Tutorial Intro

Let's discover **Docusaurus in less than 5 minutes**.

## Getting Started

Get started by **creating a new site**.

Or **try Docusaurus immediately** with **[docusaurus.new](https://docusaurus.new)**.

### What you'll need

- [Node.js](https://nodejs.org/en/download/) version 18.0 or above:
  - When installing Node.js, you are recommended to check all checkboxes related to dependencies.

## Generate a new site

Generate a new Docusaurus site using the **classic template**.

The classic template will automatically be added to your project after you run the command:

```bash
npm init docusaurus@latest my-website classic
```

You can type this command into Command Prompt, Powershell, Terminal, or any other integrated terminal of your code editor.

The command also installs all necessary dependencies you need to run Docusaurus.

## Start your site

Run the development server:

```bash
cd my-website
npm run start
```

The `cd` command changes the directory you're working with. In order to work with your newly created Docusaurus site, you'll need to navigate the terminal there.

The `npm run start` command builds your website locally and serves it through a development server, ready for you to view at http://localhost:3000/.

Open `docs/intro.md` (this page) and edit some lines: the site **reloads automatically** and displays your changes.
 -->

# Tutorial Install Vite React Tailwind by Iqmal


Halo, selamat datang di tutorial instalasi ReactJS yang disajikan oleh Iqmal! Panduan ini akan membantu Anda langkah demi langkah dalam mengatur lingkungan pengembangan untuk memulai penggunaan ReactJS.

# Panduan Instalasi ReactJS

Selamat datang di panduan instalasi ReactJS menggunakan Docusaurus! Dokumen ini akan membimbing Anda langkah demi langkah dalam mengatur lingkungan pengembangan untuk memulai proyek ReactJS Anda.

<!-- ## Persyaratan Awal

Sebelum Anda mulai menginstal ReactJS, pastikan sistem Anda memenuhi persyaratan berikut:

- Node.js: ReactJS memerlukan Node.js untuk menjalankan dan mengelola paket-paket JavaScript. Anda dapat mengunduh Node.js dari [situs resmi Node.js](https://nodejs.org/).
- npm: ReactJS menggunakan npm (Node Package Manager) untuk mengelola dependensi dan paket. npm biasanya diinstal bersamaan dengan Node.js, jadi Anda tidak perlu menginstalnya secara terpisah. -->

## Langkah-langkah Instalasi

1. **Create your project:**

   Start by creating a new Vite project if you don’t have one set up already. The most common approach is to use Create Vite.

   ```bash
   npm create vite@latest my-project -- --template react
   cd my-project
   ```

2. **Install Tailwind CSS:**

    Install tailwindcss and its peer dependencies, then generate your 'tailwind.config.js' and 'postcss.config.js' files.

    ```bash
    npm install -D tailwindcss postcss autoprefixer
    npx tailwindcss init -p
    ```
3. **Configure your template paths**
    Add the paths to all of your template files in your tailwind.config.js file.

    ```js
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

4. **Add the Tailwind directives to your CSS**
    Add the @tailwind directives for each of Tailwind’s layers to your './src/index.css' file.

    ```css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```

5. **Start your build process**
    Run your build process with 'npm run dev'.

    ```bash
    npm run dev
    ```

6. **Start using Tailwind in your project**
    Start using Tailwind’s utility classes to style your content.

    ```css
    export default function App() {
    return (
    <h1 className="text-3xl font-bold underline">
      Hello world!
    </h1>
    )
    }
    ```