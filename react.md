# React
## Get start
+ Download [nodejs](https://nodejs.org/en)  
+ Download [vscode](https://code.visualstudio.com/download)  
+ Apply *vite*  
  Create a folder in VScode and open terminal.  
+ Steps to setup vite  
>1. `npm create vite@latest`  
enter project name  
select react  
select javascript  
>2. `cd [project name]`  
>3. `npm install`  
>4. `npm run dev`  
---
## What we have now
- **node_modules** packages, library  
- **public** public assets: images  
- **src** source folder  
1. **main.jsx** contains App component from App.jsx  
2. **App.jsx** root component
3. **index.css** main css file for our application. css file imported by main.jsx
4. **App.css** css file imported by App.jsx
5. **index.html** main entrypoint into our program. It calls the main component(main.jsx) by `<script type="module" src="/src/main.jsx"></script>`  
6. **package.json** metadata for our project, project name, version, build, etc.  

As you may have seen, react works with components. And components and be inside other components.
## Practice
### Create a component
Header.jsx
```
function Header() {
  return (
    <header>
      <h1>My website</h1>
      <nav>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </nav>
      <hr />
    </header>
  );
}
export default Header
```
### Import component in App.jsx
App.jsx
```
import Header from "./Header.jsx"

function App() {
  return (
    <>
      <Header />
    </>
  );
}
```
