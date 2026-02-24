---
title: SHP to SVG Viewer
linkTitle: Visualizador de SHP para SVG
weight: 10
url: /pt/viewer/shp-to-svg/
description: Online tool for converting shapefiles to scalable vector graphics.
---

## About the Project

This project provides a web application that converts Shapefile (.shp) data into Scalable Vector Graphics (.svg) format. It allows users to upload their shapefiles and visualize them in a browser, with options to customize the appearance of features.

## Features

*   **Shapefile Upload:** Users can upload `.shp` files directly through the web interface.
*   **SVG Generation:** The application converts uploaded shapefiles into SVG format.
*   **Interactive Visualization:**  The generated SVG is displayed in an interactive viewer, allowing users to pan, zoom, and inspect features.
*   **Customization Options:** Users can adjust styling properties such as fill color, stroke color, and stroke width for different feature types.
*   **Downloadable SVG:** The resulting SVG file can be downloaded for use in other applications or platforms.

## Technologies Used

*   **Frontend:**
    *   JavaScript
    *   Leaflet (for map visualization)
    *   HTML5
    *   CSS3
*   **Backend:**
    *   Python
    *   Flask (web framework)
    *   Shapely (geometric operations)
    *   Fiona (shapefile reading/writing)

## Getting Started

### Prerequisites

*   Python 3.6 or higher
*   pip package manager

### Installation

1.  Clone the repository:

```bash
git clone [repository URL]
cd shp-to-svg-viewer
```

2.  Install dependencies:

```bash
pip install -r requirements.txt
```

### Running the Application

1.  Navigate to the project directory.
2.  Run the Flask application:

```bash
python app.py
```

3.  Open your web browser and go to `http://localhost:5000` to access the viewer.

## Usage

1.  **Upload Shapefile:** Click the "Choose File" button and select a `.shp` file from your computer.
2.  **View SVG:** The shapefile will be converted, and the resulting SVG map will be displayed in the viewer.
3.  **Customize Features (Optional):** Use the styling options to change the appearance of features on the map.
4.  **Download SVG:** Click the "Download SVG" button to save the generated SVG file to your computer.

## Contributing

Contributions are welcome! Please read the `CONTRIBUTING.md` file for guidelines on how to contribute to this project.

## License

This project is licensed under the [MIT License](LICENSE).

---

