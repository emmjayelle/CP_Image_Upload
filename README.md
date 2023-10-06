# CP Image Upload Automation

This repository contains a Python script for automating image uploads on CirclePOS Backoffice using Selenium. The script reads data from a CSV file, navigates to specific URLs, and uploads .jpg files to the corresponding elements on the webpage.

## Prerequisites

Before running the script, make sure you have the following installed:

- Python 3.x
- Selenium: `pip install selenium`
- Firefox WebDriver: [GeckoDriver](https://github.com/mozilla/geckodriver/releases)

## Usage

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/emmjayelle/CP_Image_Upload.git
   cd CP_Image_Upload

2. **Install Dependencies:**
   
```pip install -r requirements.txt```

3. **Configuration:**
Create a CSV file named input.csv with the following columns:

product_url: The target URL for each upload.

product_file: Path to the first .jpg file to upload.

product_file2: Path to the second .jpg file to upload.

product_file3: Path to the third .jpg file to upload.

product_file4: Path to the fourth .jpg file to upload.


Example input.csv:


Product URL              | Product File 1 | Product File 2 | Product File 3 | Product File 4
-------------------------|----------------|----------------|----------------|----------------
https://example.com/upload1 | file1.jpg     | file2.jpg     | file3.jpg     | file4.jpg
https://example.com/upload2 | file5.jpg     | file6.jpg     | file7.jpg     | file8.jpg

4. **Run the Script:**
   
   ```python image_upload[clean].py```

The script will automate the .jpg file upload process based on the data provided in input.csv.

**Important Notes**

Web Driver: Ensure the correct web driver is installed and compatible with your browser version.

CSV Format: Make sure the CSV file follows the specified format.

Feel free to customize the script and CSV data according to your specific use case. For any issues or improvements, please create an issue or submit a pull request.



