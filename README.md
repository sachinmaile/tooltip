# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

## Inorder to deploy the project on Netlify website follow the below steps

### In the root folder create a new file called `.netlify.toml` and append the below text
```bash
[build]
  command = "npm run build"
  publish = "/build"
  base ="/"

[[redirects]]
  from = "/*"
  to = "/index.html"
  status = 200

```

### Inside the public folder create a new file called `_redirect` and append the below text
```
/*    /index.html    200
```

### `npm run build`

Build the project 
