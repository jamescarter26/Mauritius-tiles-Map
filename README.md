Offline Map Viewer - Mauritius (MBTiles)
This project is a lightweight offline web map for Mauritius using Leaflet.js and MBTiles. It's ideal for disconnected environments, local servers (XAMPP), or embedded use where internet access is limited or unavailable.
🌍 Features
- Fully offline map of Mauritius
- Uses MBTiles (raster tiles)
- Leaflet.js for an interactive map UI
- PHP script to serve tiles from SQLite
- Simple drag-and-drop setup
📁 Project Structure

/your-project-folder
├── index.html               # Map interface
├── leaflet/                 # Leaflet.js library files
├── tiles/
│   └── mauritius.mbtiles    # Your MBTiles file (raster format)
├── php/
│   └── tile-server.php      # PHP backend to serve tiles
└── README.md                # This file

⚙️ Setup Instructions
1. Clone or Download the Repository
git clone https://github.com/your-username/offline-map-mauritius.git
2. Add MBTiles File
Place your mauritius.mbtiles inside the tiles/ folder.

📦 Download from MapTiler: https://data.maptiler.com/downloads/africa/mauritius/
🛠️ Or generate using OpenMapTiles: https://openmaptiles.org/
3. Run a Local Server
Use XAMPP or any PHP-enabled server.
Move the folder to: /xampp/htdocs/offline-map-mauritius/

Then start Apache and visit in your browser:
http://localhost/offline-map-mauritius/
🔗 Tile Server Setup (PHP)
The php/tile-server.php script handles tile delivery. Leaflet will request tiles like:
php/tile-server.php?z=10&x=512&y=340

Make sure PHP has SQLite3 enabled.
🧪 Requirements
- PHP 7+ (with SQLite support)
- Modern browser (Chrome, Firefox, etc.)
- Leaflet.js
🙏 Acknowledgements
- Map data © OpenStreetMap (https://www.openstreetmap.org/)
- Tiles via MapTiler (https://www.maptiler.com/)
- Viewer powered by Leaflet.js (https://leafletjs.com/)
🪪 License
MIT License – use freely, modify, and redistribute.
