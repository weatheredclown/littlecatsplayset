# Popsicle Party!

Welcome to **Popsicle Party!**, a fun and interactive web application where you can create your own festive scenes! Drag and drop stickers, change backgrounds, and resize items to design the perfect party setup.

## Features

- **Drag and Drop Interface**: Easily drag stickers from the tray onto the main stage.
- **Resize Items**: Select any item on the stage and use the slider to adjust its size.
- **Layering**: Click on items to bring them to the front.
- **Remove Items**: Double-click on an item to remove it from the stage.
- **Background Selection**: Choose from different backgrounds like "Beach Day" or "Garden Party" to set the mood.
- **Reset Scene**: Quickly clear the stage to start a new design.
- **Responsive Design**: Works on desktop and touch devices.

## How to Run

Because this application loads assets dynamically using `fetch`, it needs to be run on a local web server to avoid browser security restrictions (CORS) associated with the `file://` protocol.

### Using Python (Recommended)

If you have Python 3 installed, you can easily start a server:

1.  Open your terminal or command prompt.
2.  Navigate to the project directory.
3.  Run the following command:

    ```bash
    python3 -m http.server
    ```

4.  Open your web browser and go to `http://localhost:8000`.

### Other Methods

You can also use other static file servers, such as:

-   **Node.js**: `npx serve`
-   **VS Code**: Use the "Live Server" extension.

## Usage

1.  **Add Items**: Drag an item from the bottom tray onto the main stage area.
2.  **Move Items**: Click/Touch and drag an item on the stage to move it around.
3.  **Resize**: Click an item to select it (a dashed outline will appear). Use the slider that appears in the controls area to resize it.
4.  **Delete**: Double-click an item to remove it.
5.  **Change Background**: Click the "Background" button in the top control bar to select a different background image.
6.  **Reset**: Click "Reset Scene" to remove all added items and start fresh.

## Customization

The application loads its content from JSON files, making it easy to customize:

-   `assets.json`: Defines the list of stickers available in the tray.
-   `backgrounds.json`: Defines the available background options.

You can add your own images to the `images/` directory and update these JSON files to include them in the app.

## Credits

-   Assets and icons used in this project are stored in the `images/` directory.
-   Built with vanilla HTML, CSS, and JavaScript.
