# React JS {The JS library}

## DAY 1 - Introduction to React

React is a JavaScript library for building user interfaces (UIs), especially single-page applications. It allows developers to create reusable UI components and manage dynamic content effectively.

<br>

---

### Reconciliation

- React uses a virtual DOM to determine the minimal number of  DOM operations needed to update the UI.

- During reconciliation, React compares the previous virtual DOM with the new one and efficiently updates only the parts that changed.

- This makes React fast and responsive, especially for large-scale applications.

<br>

---

### SPA vs MPA

#### <u>SPA (Single Page Application)</u>

Loads a single HTML page and updates content dynamically using JavaScript.

Example: React apps, Gmail.


#### <u>MPA (Multi Page Application) </u>

Each page is a separate HTML file loaded from the server.

Example: Traditional websites, e-commerce platforms.

Pros: Better for SEO and large-scale websites with multiple pages.

---

###  **Library vs Framework**

- **Library** (like React):  
  You call the library when needed. More flexible, gives you control.

- **Framework** (like Angular):  
  The framework calls your code. It's opinionated and gives a full structure.

- **In short:**  
  > "Library is a helper, Framework is a boss."

<br>

---



####  What is NPM & Node.js?

- **Node.js**: A runtime that allows JavaScript to run outside the browser (on your machine).
- **NPM (Node Package Manager)**: Tool to install/manage packages (like React, Vite, etc.).
- React apps depend on **Node.js + NPM** to run locally and manage dependencies.

---

####  JSX & Babel

- **JSX (JavaScript XML)**: React’s syntax extension that lets you write HTML-like code inside JS.
  - JSX is not directly understood by the browser.
- **Babel**: A transpiler that converts JSX into plain JavaScript so browsers can understand it.

---

###  Import and Export in React
Components are reusable blocks. To use them across files, we need to export them from one file and import them into another.

Default Export Example:

```bash
// App.jsx
export default App;

// main.jsx
import App from './App.jsx' ;
```


#### Const /  Named Export Example:

```bash
//app.jsx
export const a = 'hellow'
export const b = 'world'

//main.jsx
import {a,b} from './App.jsx'

```


#### Setting Up a React App using Vite

- Created a folder using:
  ```bash
  //Selected React as the template.
    npm create vite@latest   

  //Installed dependencies:
    npm install

  //Ran the app locally:
     npm run dev
  ```