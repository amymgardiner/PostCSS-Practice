# PostCSS Practice

## About
The company I currently work for uses both Sass and PostCSS and I would like to become more proficient with both of them.

Kevin Powell is an educator I follow and so I watched his video on PostCSS: [Learn how to power-up your CSS with PostCSS](https://www.youtube.com/watch?v=ohJcZW60br0) and took notes and coded along.

## Notes

Post CSS
- All about the plugins! You can have it just doing one or two different things for you, or you can have it doing 25 different things.
- For example:
    - Auto-prefixing - For browser compliant code, autoprefixer is a plugin that can save you from the monotony of -webkit- and -moz- . It does exactly what it sounds like: automatically add prefixes to your CSS. All you do is supply it with a CSS sheet, and it will read through it and add vendor prefixes where needed.
    - Minifying - Minification is the process of minimizing code and markup in your web pages and script files. It's one of the main methods used to reduce load times and bandwidth usage on websites
- Once you know how to set it up, it's really easy to just plug and play all these different things that you might need on any individual project.
- This practice will use the PostCSS CLI (command-line interface), but it can be used to work with other build tools like gulp, webpack, parcel, writing your own npm scripts. etc.

File Organization
- One main CSS stylsheet with several other smaller CSS files - One single file for production, but can break it down while working on it and make it easier to find styles and maintain the code.
- Similar to Sass functionality.
- Kevin has another video about organization: [Get your stylesheets more organized with Sass partials](https://www.youtube.com/watch?v=9Ld-aOKsEDk)

Import
- Different from the [CSS Import Rule](https://www.w3schools.com/cssref/pr_import_rule.php), which is not recommended to use as it slows things down.
- PostCSS Import takes all of the seperate stylesheets and combines them all into one, and outputs a single file that would go into a distribution, public, etc. folder (the final production folder).
- The production folder goes onto the server, but the seperate stylsheets are the dev environment which is a bit different.
- The next step after postcss.config.js and style.css, would be to go into the package.json file to add a new script to tell PostCSS what to do, where to go, and what to output. This is how we get it to import everything together.