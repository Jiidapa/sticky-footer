## Stick Footer with Bootstrap

ยึด concept คือ
```html
<html>
    <header>
        <style>
            html, body {
                height: 100%;
                margin: 0;
            }
            .content {
                min-height: 100%;
                margin: 0 auto -50px;
            }
            .footer {
                height: 50px;
            }

            footer {
                background: #42A5F5;
                color: white;
                line-height: 50px;
                padding: 0 20px;
            }

        </style>
    </header>
    <body>
        <div class="content"></div>
        <footer class="footer">my sticky footer</footer>
    </body>
</html>
```

แปลงเป็น sticky ของ react โดยใช้ bootstrap
1. ใน html tag ใส่ class="h-100"

```html
// public/index.html
<html class="h-100"></html>
```

2. ใน body ใส่ class="h-100"
```html
// public/index.html
<html class="h-100">
    <body class="h-100"></body>
</html>
```

3. ใน div id="root" ใส่ class="d-flex flex-column h-100"
```html
// public/index.html
<html class="h-100">
    <body class="h-100">
        <div id="root" class="d-flex flex-column h-100"></div>
    </body>
</html>
```
4. ใน component footer ใส่ className="footer mt-auto"
```html
// public/index.html
<footer className="footer w-100">
    <p className="my-0">© Hostel Management { new Date().getFullYear() }</p>
</footer>
```



This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
