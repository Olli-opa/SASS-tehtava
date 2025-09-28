# Bistro Aurora

## Project Overview
Bistro Aurora is a simple website project built using HTML and Sass. The website serves as an online presence for a fictional restaurant, showcasing its offerings and providing essential information to visitors.

## Project Structure
```
bistro-aurora
├── index.html          # Main HTML document for the website
├── scss                # Directory containing Sass files
│   ├── _variables.scss # Sass variables for colors, typography, and measurements
│   ├── _mixins.scss    # Mixin definitions for reusable styles
│   ├── _layout.scss    # Layout styles for the website
│   └── style.scss      # Main entry point for importing all partials
├── css                 # Directory for compiled CSS files
│   └── style.css       # Compiled CSS output from the Sass files
└── README.md           # Documentation for the project
```

## Features
- **Responsive Design**: The website is designed to be responsive, adapting to various screen sizes using media queries.
- **Reusable Styles**: Sass mixins are used to create reusable styles for buttons and containers, promoting consistency across the site.
- **Customizable Variables**: Sass variables allow for easy customization of colors, typography, and spacing throughout the project.

## Setup Instructions
1. Clone the repository:
   ```
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```
   cd bistro-aurora
   ```
3. Install the necessary dependencies for Sass (if using a package manager):
   ```
   npm install
   ```
4. Compile the Sass files to CSS:
   ```
   sass scss/style.scss css/style.css
   ```
5. Open `index.html` in your web browser to view the website.

## Usage
Feel free to modify the Sass variables and mixins to customize the look and feel of the website. Add additional content to `index.html` as needed to expand the site’s offerings.