# Service Worker Listeners

This project is a simple Progressive Web App (PWA) created to demonstrate the functionality of different event listeners in a Service Worker.

## Features

The Service Worker in this project (`sw.js`) is configured to listen for the following events:

- `install`: Triggered when the Service Worker is first installed. This is where assets can be pre-cached.
- `activate`: Triggered when the Service Worker is activated. This is a good place to clean up old caches.
- `fetch`: Triggered for every network request made by the page. This allows for intercepting requests and implementing caching strategies.
- `sync`: Triggered when the browser regains connectivity. This is used for background synchronization tasks.
- `push`: Triggered when a push notification is received from a server.

## Project Structure

- `index.html`: The main HTML file for the PWA.
- `sw.js`: The Service Worker file containing all the event listeners.
- `js/app.js`: The main JavaScript file that registers the Service Worker.
- `css/style.css`: Basic styles for the application.
- `img/`: Contains the images used in the application.

## How to Use

To run this project, you need to serve the files using a local web server. A simple way to do this is by using Python's built-in HTTP server.

1.  Navigate to the project's root directory in your terminal.
2.  Run the following command:

    ```bash
    python -m http.server
    ```

3.  Open your web browser and go to `http://localhost:8000`.

You can then open the browser's developer tools to see the console logs from the Service Worker.
