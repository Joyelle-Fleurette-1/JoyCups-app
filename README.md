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
9. Eslint for code linting
   1. Install VScode eslint extension 
   2. npm install -D eslint --registry http://registry.npmjs.org/ for code linting
   3. Run ./node_modules/.bin/eslint --init
   4. npm install eslint-plugin-react@latest --save --registry http://registry.npmjs.org/
   5. Re-run ./node_modules/.bin/eslint --init the error will be fixed
   6. Create ./frontend/.env and add SKIP_PREFLIGHT_CHECK=true
10. Add redux to Home Screen to manage the state of our react application
   1. npm install redux react-redux
   2. Create store.js
   3. initState= {products:[]}
   4. reducer = (state, action) => switch LOAD_PRODUCTS: {products: action.payload}
   5. export default createStore(reducer, initState)
   6. Edit HomeScreen.js
   7. shopName = useSelector(state=>state.products)
   8. const dispatch = useDispatch()
   9. useEffect(()=>dispatch({type: LOAD_PRODUCTS, payload: data})
   10. Add store to index.js
11. Add Redux to Product Screen
   1. create product details constants, actions and reducers
   2. add reducer to store.js
   3. use action in ProductScreen.js
   4. add /api/product/:id to backend api
   5. npm install redux-thunk --registry http://registry.npmjs.org/
12. Handle Add To Cart Button
   1. Handle Add To Cart in ProductScreen.js
   2. create CartScreen.js
13. Implement Add to Cart Action
   1. create addToCart constants, actions and reducers
   2. add reducer to store.js
   3. use action in CartScreen.js
   4. render cartItems.length
14. Build Cart Screen
   1. create 2 columns for cart items and cart action
   2. cartItems.length === 0 ? cart is empty
   3. show item image, name, qty and price
   4. Proceed to Checkout button
   5. Implement remove from cart action
15. Implement Remove From Cart Action
   1. create removeFromCart constants, actions and reducers
   2. add reducer to store.js
   3. use action in CartScreen.js
16. Create Sample Users In MongoDB
   1. npm install mongoose
   2. npm install bcrypt for password security
   3. connect to mongodb
   4. create config.js
   5. npm install dotenv
   6. export MONGODB_URL
   7. create models/userModel.js
   8. create userSchema and userModel
   8. create userRoute
   9. Seed sample data
17. Create Sample Products In MongoDB
   1. create models/productModel.js
   2. create productSchema and productModel
   3. create productRoute
   4. Seed sample data
18. Create Sign-in Backend
   1. create /signin api
   2. check email and password
   3. generate token
   4. install json web token
   5. install dotenv
   6. return token and data
   7. test it using postman
19. Design SignIn Screen
   1. create SigninScreen
   2. render email and password fields
   3. create signin constants, actions and reducers
   4. Update Header based on user login
20. Implement SignIn Action
   1. create signin constants, actions and reducers
   2. add reducer to store.js
   3. use action in SigninScreen.js
21. Create Register Screen
   1. create API for /api/users/register
   2. insert new user to database
   3. return user info and token
   4. create RegisterScreen
   5. Add fields
   6. Style fields
   7. Add screen to App.js
   8. create register action and reducer
   9. check validation and create user
22. Create Shipping Screen
   1. create CheckoutSteps.js component
   2. create shipping fields
   3. implement shipping constant, actions and reducers
23. Create Payment Screen
   1. create payment fields
   2. implement shipping constant, actions and reducers
24. Design Place Order Screen
   1. design order summary fields
   2. design order action
25. Create Place Order API
   1. createOrder api
   2. create orderModel
   3. create orderRouter
   4. create post order route
26. Implement PlaceOrder Action
   1. handle place order button click
   2. create place order constants, action and reducer
27. Create Order Screen
   1. build order api for /api/orders/:id
   2. create OrderScreen.js
   3. dispatch order details action in useEffect
   4. load data with useSelector
   5. show data like place order screen
   6. create order details constant, action and reducer