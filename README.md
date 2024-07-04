# Camera Feed for Google Cardboard

## Motivation / Use Case
This application is designed to help individuals who need to perform tasks requiring eye protection, such as arc soldering, by allowing them to see through the camera of their phone while wearing Google Cardboard goggles. The application captures the camera feed and splits it into two halves, providing a stereoscopic view that can be used with Google Cardboard goggles for enhanced safety and visibility.

## Technical Description
This single-page application (SPA) uses HTML, CSS, and JavaScript to capture the device's camera feed and display it on a canvas that is split into two parts. The layout is fixed to landscape mode to ensure compatibility with Google Cardboard goggles. The application uses the `navigator.mediaDevices.getUserMedia` API to access the camera and display the live feed.

### Key Components:
- **HTML**: Structure of the page, including the canvas split into two halves.
- **CSS**: Styling to ensure the application takes up the full screen and stays in landscape mode.
- **JavaScript**: Logic to capture and display the camera feed in real-time.

## Instructions on How to Load/Run

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/yourusername/camera-feed-cardboard.git
    cd camera-feed-cardboard
    ```

2. **Serve the Application**:
    You need to serve the files using a local server. You can use any file server, such as `http-server` or Python's built-in HTTP server.

    - Using `http-server` (Node.js):
        ```sh
        npx http-server .
        ```

    - Using Python (Python 3.x):
        ```sh
        python -m http.server
        ```
    - using github directly
       open this link in your browser:
         [https://raw.githubusercontent.com/alfu32/arc-solder-google-goggles/work/index.html]
         or
         [https://alfu32.github.io/arc-solder-google-goggles/]
3. **Open the Application**:
    Open your web browser and navigate to `http://localhost:8080` (the port might differ if you use a different server).

4. **Use the Application**:
    - Ensure your device is in landscape mode.
    - Place your phone inside the Google Cardboard goggles.
    - Grant camera access when prompted.
    - The camera feed will be displayed on the split canvas, providing a stereoscopic view.

Enjoy using the application for a safer and more efficient soldering experience!
