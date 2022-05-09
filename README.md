# Angular Server Side Rendering

This project demonstrates how server side rendering is achieved in Angular framework. When a web page is loaded on the browser usually the initial files like index.html, main.js and styles.css are being fetched separately and displayed by the browser. In server side rendering Angular universal creates a static page upon request and sends it to the client (Browser) in the initial request. This will display the first-contentful paint faster, which makes the loading of website faster for both user and a web crawler to rank the websites. This will result in some time required to initially interact with the page until the actual bundles are fetched from the server.

## Running the application

Run `npm run dev:ssr` for a dev server. Navigate to `http://localhost:4201/`. The app will automatically reload if you change any of the source files.

## Testing the Server side rendering

Inspect the webpage once after the server is up and running. Navigate to networks tab and check the preview of initial network call to the server. It displays the static page which was generated on request. This is not the case when the application is run normally using `ng serve`.

## Build the application

Run `ng build && ng run app-name:server` to build both the server script and the application in production mode. Use this command when you want to build the project for deployment.

## Further details

To get more details on the Angular Server side rendering go check out the [Server-side rendering (SSR) with Angular Universal](https://angular.io/guide/universal) page.
