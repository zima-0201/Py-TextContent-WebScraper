# Web Scraping and Text Extraction Script

This script is designed to automate the process of logging into a website, navigating through specified links, and extracting text content from subpages. It utilizes the requests library for making HTTP requests, BeautifulSoup for parsing HTML, and the os library for file and folder manipulation.

## Video Preview

[![Video Preview](https://github.com/DevRex-0201/Project-Images/blob/main/video%20preview/Py-TextContent-WebScraper.png)](https://drive.google.com/file/d/13BddvUnbY034azQJGQ2FwnxFBIpwR8yT/view?usp=drive_link)

## Requirements

Ensure you have the required Python libraries installed. You can install them using the following command:

```bash
pip install requests beautifulsoup4
```

## Usage

1. Modify the script with your specific details:

   - `site_url`: The base URL of the website.
   - `login_url`: The URL for logging into the website.
   - `page_url`: The URL of the main page containing links to be processed.
   - `loginname`: Your login username.
   - `password`: Your login password.
   - `links`: A list of specific subpage URLs from which to extract text.

2. Run the script:

   ```bash
   python script_name.py
   ```

## Script Explanation

1. **Login Process:**
   - The script creates a session, logs in using the provided credentials, and handles any login errors.

2. **Text Extraction:**
   - The script then iterates through a list of specified subpage URLs.
   - For each subpage URL, it makes a request, parses the HTML with BeautifulSoup, and extracts text content from elements within a div with the class "wpb-content-wrapper."
   - The extracted text is then saved to a text file.

3. **Folder Structure:**
   - The script saves each text file with a filename based on the subpage URL, ensuring uniqueness.

## Important Notes

- This script is provided as a starting point and may require adjustments based on the specific structure and behavior of the target website.

- Ensure compliance with the website's terms of service and legal requirements before using or modifying the script.

- Handle login credentials securely, considering encryption or other secure practices.

- Use responsibly and avoid excessive requests to the website to prevent potential issues.

## Disclaimer

This script is provided for educational purposes and may need customization to work with specific websites. Use it responsibly and respect the website's terms of service. The author is not responsible for any misuse or legal consequences resulting from the use of this script.
