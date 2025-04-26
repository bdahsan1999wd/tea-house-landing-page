## ✅ Tailwind CSS v4 CLI Setup: Quick & Simple Guide

Follow these steps to set up Tailwind CSS v4 using the CLI method.

1.  ✅ **Install Tailwind CSS**

    Install Tailwind CSS and its CLI tool using npm:

    ```bash
    npm install tailwindcss @tailwindcss/cli
    ```

2.  ✅ **Import Tailwind in your CSS Create a CSS file (e.g., src/input.css) and import Tailwind**

    ```css
    @import "tailwindcss";
    ```

    ```bash
    npm install tailwindcss@latest @tailwindcss/cli@latest daisyui@latest
    ```

3.  ✅ **Configure package.json Add a build script to your package.json**

    ```json
    {
      "scripts": {
        "build": "npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch"
      }
    }
    ```

4.  ✅ **Build the CSS Run the following command to start generating your Tailwind Output**

    ```bash
    npm run build
    ```

5.  ✅ **Link the Compiled CSS in HTML In your src/index.html, link the generated CSS**

    ```html
    <!DOCTYPE html>
    <html lang="en">
      <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Tailwind CSS CLI</title>
        <link href="./output.css" rel="stylesheet" />
      </head>
      <body></body>
    </html>
    ```

6.  ✅ **.gitignore Tips:**

    A `.gitignore` file specifies which files and directories should _not_ be included in your Git repository. This keeps your repository clean and avoids committing unnecessary files.

    Add the following to your `.gitignore` file:

    ```
    node_modules
    ```

    `node_modules`: This directory contains the Node.js packages you've installed. It can be huge and should not be committed.

    After cloning the project, use these commands:

    ```bash
    npm install     # Reinstalls the packages listed in package.json
    npm run build   # Regenerates the output.css file
    ```

7.  ✅ **Final Step:** Open `src/index.html` in your browser and enjoy Tailwind CSS in action!
