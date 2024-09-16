# Brainwave-Template

Team Brainwave's template repo from FAC30

### Recommended folder structure (delete what is not applicable)

Here is a recommended folder structure:

```
/project-root
│
├── /assets
│   ├── /fonts          # Font files
│   ├── /images         # Image files
│   ├── /icons          # Icon files
│   └── /videos         # Video files
│
├── /css
│   ├── root.css        # Main style sheet linking stylesheets below
│   ├── README.md       # Style documentation
│   ├── /base           # Base styles (resets, typography)
│   │   └── reset.css   # CSS reset or normalize
│   │   └── typography.css # Base typography styles
│   ├── /components     # Component-specific styles (buttons, cards, etc.)
│   │   └── button.css
│   │   └── card.css
│   ├── /layout         # Layout styles (grid, flexbox)
│   │   └── grid.css
│   │   └── flexbox.css
│   │   └── header.css
│   │   └── footer.css
│   │   └── navbar.css
│   │   └── media-queries.css
│   ├── /pages          # Page-specific styles (home, about)
│   │   └── home.css
│   │   └── about.css
│   │   └── services.css
│   │   └── contact.css
│
├── /js
│   ├── main.js         # Main JavaScript file
│   ├── server.js       # Express.js server setup
│   └── README.md       # JavaScript documentation
│
│
├── index.html          # Main HTML file
├── README.md           # Project documentation (this file)
├── package.json        # Node package file
├── .gitignore          # Gitignore file - must contain .env!
└── .env                # Environment file containing authentication secrets
```

### Key Elements and Best Practices for `.html` file:

1. **DOCTYPE**: Declares the document type and version of HTML.
2. **`<meta charset="UTF-8">`**: Ensures the document is interpreted with the correct character set.
3. **Responsive Meta Tag**: `viewport` meta tag for responsive design on mobile devices.
4. **SEO and Social Sharing**: Includes meta tags for description, keywords, and Open Graph protocol.
5. **Semantic HTML5 Elements**: Uses `<header>`, `<nav>`, `<main>`, `<section>`, and `<footer>` for better structure and accessibility.
6. **Accessibility Considerations**: Proper use of headings (`<h1>`, `<h2>`, etc.) and descriptive link text.
7. **CSS and JavaScript**: Linked external stylesheets and scripts for better performance and maintainability.

Feel free to customize the content, structure, and links to suit your needs!

Here's a basic `.env` template for storing environment variables. This file is typically used to keep sensitive information like API keys, database credentials, and other configuration details that should not be hardcoded in your application code.

### Key Elements and Best Practices for `.env` file

1. **Keep It Secure**: Never share your `.env` file in a public repository. Add the `.env` file to your `.gitignore` to prevent it from being committed to version control.
2. **Environment-Specific Configurations**: Use different `.env` files for different environments (e.g., `.env.development`, `.env.production`) to handle environment-specific configurations.
3. **Use Descriptive Names**: Name your environment variables clearly and consistently. Prefix them if necessary to indicate their purpose (e.g., `DB_`, `API_`, `JWT_`).
4. **Avoid Hardcoding Secrets**: Store sensitive information like passwords, API keys, and tokens in your `.env` file, not in your source code.
5. **Load Variables Properly**: Use a library like `dotenv` in Node.js or similar libraries in other environments to load the `.env` file's variables into your application.

This template should cover the common types of configurations needed in a project, and you can adjust it according to your specific use case.