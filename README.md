# How to initialize the Tailwind in HTML
- npm install -D tailwindcss
- npx tailwindcss init

# In tailwind config file
- module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}

# Create new file input.css
- @tailwind base;
- @tailwind components;
- @tailwind utilities;

# To Track what we are changing in the code Tailwind want the CLI build process to keep track.
- npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch