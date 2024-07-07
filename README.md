# Tailwind

Hi, i want to leave this easy track to how add Tailwind to your project.

### Open Terminal:

**Type:**

```powershell
cd "The folder where you want to create the project"
```

```powershell
npm create vite@latest "Name of the project 'Folder' "
```

**One time created open the folder on Vscode**

**Type in the terminal:**

```powershell
npm install -D tailwindcss postcss autoprefixer
```

```powershell
npx tailwindcss init -p
```

**Insert that on the `tailwind.config.js` file.**

```jsx
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

**Insert that on the `./src/index.css` file.**

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

**To run the project type:**

```powershell
npm run dev
```

**Start using Tailwind in your project:**

```html
<div id="div" class="flex flex-grow flex-col justify-between items-center text-center min-h-screen scroll-smooth">
      <div class="flex justify-center items-center text-center min-h-90vh w-screen">
        <h1 class="text-black">
          Get Your Next
        </h1>
      </div>
      <div class="flex justify-center text-center items-center w-screen bg-yellow-200">
        <a href="">
          <div class="flex justify-center text-center items-center h-16 min-w-full bg-yellow-200">
            <h1 class="text-black flex text-center items-center">
              Here's how it works
              
              <div class="animate-bounce">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="size-5">
                  <path fill-rule="evenodd" d="M5.22 8.22a.75.75 0 0 1 1.06 0L10 11.94l3.72-3.72a.75.75 0 1 1 1.06 1.06l-4.25 4.25a.75.75 0 0 1-1.06 0L5.22 9.28a.75.75 0 0 1 0-1.06Z" clip-rule="evenodd" />
                  </svg>
              </div>
            </h1>
          </div>
        </a>
      </div>
    </div>
```
