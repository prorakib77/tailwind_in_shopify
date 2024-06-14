# tailwind_in_shopify

1: npm init -y
2: npm install -D tailwindcss
3: npx tailwindcss init
4: customized the tailwind.config.js file -
	/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    '.layout/*.liquid',
    '.section/*.liquid',
    '.snippets/*.liquid'
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}





5: create a folder and inside file called - src -> tailwind.css
6: write the - 
@tailwind base;
@tailwind components;
@tailwind utilities;
Code inside the tailwind.css file
7: Firstrun this command - npx tailwindcss -i ./src/input.css -o ./src/output.css
8: Create .shopifyignore file
Write -> 
package.json
package-lock.json
css
node_modules

9:Then -> npx tailwindcss -i ./src/tailwind.css -o ./assets/main.css --watch

Done

