https://simplystellar.au

This is a website built using entirely HTML/CSS and JS without the use of any frameworks or page-builders. It's compliant with WCAG 2.1 and is responsive across all screen sizes. I utilise the LESS preprocessor, and have a folder script to optimise all images into webp.

The project structure includes several folders at the root level, such as .eleventy.js, .gitignore, and package.json. The .eleventy.js file is the main configuration file for Eleventy, where you can optimise images, define component locations, and specify files for the production build. The other folders, like node_modules and public, are for dependencies and the production-ready code, respectively.

You primarily work in the src folder, which contains the organised system for building your website. The _data folder stores global data that can be accessed throughout the project. The _includes and _layouts folders contain reusable components and page layouts, respectively. The admin folder holds configuration files for the CMS, and the assets folder is for non-HTML/CSS assets like JavaScript and images. The blog folder stores blog post markdown files, and the CSS folder contains LESS and CSS files. The images folder has images to be optimized, while assets/images stores images that don't require optimization.

The reason for having two image folders is related to the Eleventy image plugin. Images in src/images are optimized and saved to the /public build folder, while assets/images contains images that don't undergo optimization. CMS images cannot be optimized by Eleventy, and certain images like the logo may not need resizing or optimization, so they reside in assets/images.
