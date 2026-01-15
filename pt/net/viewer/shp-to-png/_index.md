---
title: SHP to PNG Viewer
linkTitle: Visualizador de SHP para PNG
weight: 10
url: /pt/viewer/shp-to-png/
description: Convert SHP files to PNG images with this simple viewer.
---

## About the Project

This project provides a simple web application for converting Shapefile (SHP) files into Portable Network Graphics (PNG) images. It allows users to upload an SHP file and generate a preview image, which can then be downloaded.

## Features

*   Upload SHP files
*   Generate PNG previews
*   Download generated images
*   Simple and user-friendly interface

## Technologies Used

*   Python
*   Flask
*   Shapely
*   GDAL
*   PIL (Pillow)

## Getting Started

### Prerequisites

Make sure you have the following installed:

*   Python 3.6 or higher
*   pip

### Installation

1.  Clone the repository:

    ```bash
    git clone [repository URL]
    cd shp-to-png-viewer
    ```

2.  Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

### Running the Application

1.  Navigate to the project directory.
2.  Run the Flask application:

    ```bash
    python app.py
    ```

3.  Open your browser and go to `http://127.0.0.1:5000/` to access the viewer.

## Usage

1.  Upload an SHP file using the upload button.
2.  The application will automatically generate a preview image.
3.  Click the "Download" button to download the PNG image.

## Contributing

Feel free to contribute to this project by submitting pull requests or reporting issues.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

If you have any questions or suggestions, please contact us at [your email address].
---
