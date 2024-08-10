# Where in the World is Naren

This project is an interactive map that showcases all the places around the world where I have traveled or lived in. It uses Leaflet.js for map rendering and allows me to mark specific locations with pins. The last place in the list of locations is highlighted as my current location.

## Features

- **Interactive Map:** Explore the map with zooming and panning capabilities.
- **Markers:** Pins are placed on the map to indicate each location.
- **Current Location:** The last place in the list is highlighted as the current location.
- **Zoom Restrictions:** The map prevents zooming out beyond the world view, ensuring a controlled user experience.
- **Responsive Design:** The map is fully responsive and adjusts to different screen sizes.

## Technologies Used

- **Leaflet.js:** A popular open-source JavaScript library for mobile-friendly interactive maps.
- **HTML/CSS/JavaScript:** The standard web technologies used to structure and style the project.
- **GitHub Pages:** Used to host and deploy the project.

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   ```

2. **Navigate to the project directory:**
   ```bash
   cd <your-repo-name>
   ```

3. **Open `index.html` in your browser:**
   - You can simply double-click `index.html` to open it, or use a local server to view it in the browser. BUT this will not show places because of CSRF issues. Use the methods below instead. 

   **Using Python's SimpleHTTPServer:**
   ```bash
   python3 -m http.server
   ```

   **Using Node.js with http-server:**
   ```bash
   npm install -g http-server
   http-server
   ```

4. **Explore the Map:**
   - Once the project is running, you can explore the map and see all the places marked with pins.

## Adding New Locations

To add new locations:

1. Open the `places.json` file.
2. Add a new entry with the following format:
   ```json
   {
       "name": "New Location, Country",
       "coords": [latitude, longitude]
   }
   ```
3. Save the file and refresh the map to see the new location.

## Deployment

This project is deployed using GitHub Pages. To deploy:

1. Push your latest changes to the `main` branch (or the branch you use for deployment).
2. Enable GitHub Pages in the repository settings by selecting the `main` branch as the source.
3. Your project will be live at `https://<your-username>.github.io/<your-repo-name>/`.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Credits

- **Leaflet.js**: For providing an excellent open-source mapping library.
- **OpenStreetMap**: For the map tiles used in this project.