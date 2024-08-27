# Media Dashboard

This repository contains a Streamlit application that interacts with Cloudinary to upload, tag, and manage images. The application provides functionalities for viewing images in a gallery and analyzing tag statistics.

## Features

- **Upload and Tag Images**: Automatically upload images to Cloudinary and tag them using OpenImages.
- **Image Gallery**: Browse uploaded images by their tags in a visually appealing gallery format.
- **Image Statistics**: Analyze the frequency of tags and the most common combinations of tags using interactive visualizations.

## Installation

### Prerequisites

- Python 3.7 or higher
- Cloudinary account

### Setup

1. Clone the repository:

   ```
   git clone https://github.com/muhammedozmen/MediaDashboard.git
   cd MediaDashboard

   ```

2. Create and activate a virtual environment:

   ```
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

   ```

3. Install the required packages:

   ```
   pip install -r requirements.txt
   ```

4. Set up your environment variables:
   
   Create a .env file in the project root directory and add your Cloudinary URL:
   ```
   CLOUDINARY_URL=cloudinary://your_cloudinary_key:your_cloudinary_secret@your_cloudinary_cloud_name
   ```

5. Run the application:

   ```
   streamlit run app.py
   ```

## Usage

### Upload Images

You can upload images to Cloudinary using the cloudinary_service.py script. The images will be automatically tagged and organized under the specified folder.

### Image Gallery

Browse through your images using the Image Gallery option. You can filter images by tags or tag combinations.

### Image Statistics

Analyze the tags of your images with interactive charts under the Image Stats option. View the most frequent tags and common tag combinations.

## Code Overview

- `cloudinary_service.py`: Contains functions for interacting with Cloudinary, including uploading images, tagging, and retrieving images with tags.
- `app.py`: The main Streamlit application that provides a user interface for viewing images and statistics.
- `.env`: Stores environment variables, particularly the Cloudinary URL.

## Dependencies

- `streamlit`: For creating the web application.
- `cloudinary`: For interacting with the Cloudinary API.
- `plotly`: For generating interactive plots and charts.
- `pandas`: For data manipulation and analysis.
- `python-dotenv`: For managing environment variables.

## Contributing

Contributions are welcome! Please fork this repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

If you have any questions or suggestions, feel free to reach out via GitHub issues or LinkedIn.
