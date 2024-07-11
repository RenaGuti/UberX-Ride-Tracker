# UberX-Ride-Tracker
This project downloads detailed information about UberX rides, including payment, time, and other relevant data. The primary goal is to facilitate subsequent analysis and strategy development for drivers, particularly focusing on increasing their profitability.

## Prerequisites

- Python 3.x
- Selenium
- ChromeDriver (compatible with your version of Chrome)

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/RenaGuti/uber-earnings-scraper.git
   cd uber-earnings-scraper

## Usage
Initial Setup
Ensure you have your Uber driver account credentials ready.

Modify the driver_path in the script to the path where you have placed the ChromeDriver executable:

driver_path = 'path/to/your/chromedriver'
Running the Script.

Automated Login:

Run the script:

python uber_earnings_scraper.py
The script will attempt to navigate to the Uber earnings activities page and log in automatically. If the login is successful, it will start extracting the data.

Manual Login:

If the script fails to log in due to extra security measures (e.g., captcha, two-factor authentication), follow these steps:

Manually open Chrome and log in to your Uber driver account.
Navigate to the earnings activities page.
Once logged in and the page is fully loaded, close the browser.
Re-run the script, and it will detect the active session and continue with data extraction.

## Data Extraction
The script will extract the following data for each entry in the earnings activities table:

Event
Date
Time
Earnings
The extracted data will be printed in the console. You can modify the script to save the data to a file if needed.

## Script Overview
The script uses Selenium to automate the login process (if needed) and to navigate to the earnings activities page. It then extracts the data using XPath selectors to ensure that all relevant information is captured accurately.

This project is focused on obtaining the driving data from Uber drivers in order to improve the strategies they use. By analyzing the data, drivers can gain insights into their performance and make informed decisions to enhance their earnings and efficiency.

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an Issue to discuss any changes or improvements.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

