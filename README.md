# JoyCups Ecommerce Website
1. Build the template for the website
   1. Create JoyCups folder
   2. create template folder
   3. create index.html and style.css files
   4. add default HTML code
   5. link index.html to style.css
   6. create header, main and footer
   7. style elements
2. Display Products
   1. create products div
   2. add product attributes
   3. add link, image, name and price
3. Create React App
   1. npx create-react-app frontend
   2. npm start
   3. Remove unused files
   4. copy index.html content to App.js
   5. copy style.css content to index.css
   6. replace class with className
4. Share Code On Github
   1. Initialize git repository
   2. Commit changes
   3. Create repo on github
   4. Create a new SHH key and add it on Github
   5. connect local repo to github repo
   6. push changes to github
5. Create Rating and Product Component
   1. create components/Rating.js
   2. create div.rating
   3. style div.rating, span and last span
   4. Create Product component
   5. Use Rating component
6. Build Product Screen
   1. Install react-router-dom
   2. Use BrowserRouter and Route for Home Screen
   3. Create HomeScreen.js
   4. Add product list code there
   5. Create ProductScreen.js
   6. Add new Route from product details to App.js
   7. Create 3 columns for product image, info and action
7. Create Node.JS Server
   1. run npm init in root folder
   2. Update package.json set type: module
   3. Add .js to imports
   4. npm install express
   5. create server.js
   6. add start command as node backend/server.js for rerun whenever there is a change
   7. require express
   8. create route for / return backend is ready.
   9. move products.js from frontend to backend
   10. create route for /api/products
   11. return products
   12. run npm start
   13. npm install --save-dev nodemon --registry http://registry.npmjs.org/
8. Load Products From Backend
   1. add "proxy": "http://127.0.0.1:5000" in frontend package.json
   2. cd frontend and npm install axios --registry http://registry.npmjs.org/
   3. edit HomeScreen.js
   4. define products, loading and error.
   5. create useEffect
   6. define async fetchData and call it
   7. get data from /api/products
   8. show them in the list
   9. create Loading Component
   10. create Message Box Component
   11. use them in HomeScreen
9. 1. install VScode eslint extemsion 
   2. npm install -D eslint --registry http://registry.npmjs.org/ for code linting
   3. Run ./node_modules/.bin/eslint --init
   4. npm install eslint-plugin-react@latest --save --registry http://registry.npmjs.org/
   5. Re-run ./node_modules/.bin/eslint --init the error will be fixed
   6. 
