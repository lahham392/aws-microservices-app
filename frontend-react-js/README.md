# Frontend React JS

## Waht is React.js ???

React.js is a JavaScript library for building user interfaces, 
primarily focused on the frontend or client-side of web applications. 
When working with React, you typically structure your files and directories in
a specific way to organize your components, assets, and other related files.


## Common structure of React.js projects
``` 
my-react-app/
├── node_modules/
├── public/
│   ├── index.html
│   ├── favicon.ico
│   └── ...
├── src/
│   ├── components/
│   │   ├── Header.js
│   │   ├── Footer.js
│   │   ├── ProductList.js
│   │   └── ...
│   ├── pages/
│   │   ├── HomePage.js
│   │   ├── ProductPage.js
│   │   └── ...
│   ├── utils/
│   │   ├── helpers.js
│   │   └── ...
│   ├── assets/
│   │   ├── images/
│   │   ├── styles/
│   │   │   ├── global.css
│   │   │   └── ...
│   │   └── ...
│   ├── App.js
│   ├── index.js
│   └── ...
├── .gitignore
├── package.json
├── package-lock.json
└── ...

```

## Used in this project

### public/
This directory contains the static files that will be served by the web server, such as the index.html file, which is the entry point of your React application, and other assets like images and favicon.

1. **index.html:** This is the main HTML file that serves as the entry point for your React application. 

2. **favicon.ico:** This is the icon that will be displayed in the browser tab or bookmark for your application.

3. **robots.txt:** This file is used to provide instructions for web crawlers and search engine bots about which pages or files should be crawled or ignored.

4. **browserconfig.xml:** it provides instructions to Microsoft browsers on how to display and configure the tile (icon) for a website or web application that has been pinned to the Start menu or taskbar.
The <tile> element defines the configuration for the tile (icon) that will be displayed when the website is pinned.
    **square150x150logo src="mstile-150x150.png"/>:** This specifies the path to the 150x150 pixel PNG image that should be used as the tile icon for the pinned website.
    **TileColor>#da532c TileColor>:** This sets the background color of the tile to the specified hexadecimal color value (#da532c, which is a reddish-orange color).

5. **safari-pinned-tab.svg:** is a file used to customize the appearance of a website or web application when pinned or opened as a tab in Apple's Safari browser on macOS and iOS.

6. **site.webmanifest:** is a JSON file that provides metadata about a web application, allowing it to be installed and run as a Progressive Web App (PWA) on various platforms and devices.
The web app manifest file provides information about the application, such as its name, icons, start URL, display mode, and more. This metadata is used by browsers and operating systems to determine how the web app should be displayed and behaved when launched or installed.

### src/
This is the main directory where you'll find the written React code.

#### components/
This directory usually contains reusable React components that can be used across multiple pages or other components. Components are the building blocks of a React application, and they encapsulate UI logic and functionality.

Each component typically has a .js (or .jsx) file for the component code and a .css (or styled-components) file for styles.


#### pages/
his directory contains the top-level components that represent full pages or views in the application. Like components, each page is often organized into its own subdirectory with a .js (or .jsx) file for the page component and a .css file for styles specific to that page.

#### App.js
This is the root component of your React application, where you define the main layout, routing, and potentially import other top-level components or providers.

#### index.js
This is the entry point of your React application, where the root component (App.js) is rendered and attached to the DOM.

The DOM (Document Object Model) is a programming interface that represents the structure of a web page and allows you to manipulate its elements using JavaScript. In the context of React, the index.js file is where you instruct React to render your components by targeting a specific element in the DOM (in your case, the <main> element) and rendering your root component (<App />) inside it.

We don’t really touch the index.js file at all.
That is just a place to render the app.
I will write my code in the app.js or write code in separate components and then nest them inside the app.js

