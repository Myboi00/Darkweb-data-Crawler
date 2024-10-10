# Darkweb-data-Crawler
Tor-Enabled Onion Website Scraper with Keyword Analysis is a Python-based web scraping tool designed to search and analyze .onion websites over the Tor network. This project enables users to access hidden services that are not reachable through standard web crawlers due to the unique .onion domain and the need for a Tor proxy.

Key Features
Tor Network Integration: This scraper fully supports the Tor network, allowing access to hidden services that traditional web scrapers cannot reach. Many crawlers are limited to the surface web and cannot navigate the complexities of the dark web.

Keyword Analysis: The tool not only fetches URLs but also analyzes the content of each page to count occurrences of a user-defined keyword. This functionality is essential for users who want to gather data related to specific topics on the dark web.

Excel Data Storage: Results are automatically saved in Excel format, making it easy for users to review and analyze the scraped data later. This feature streamlines the process of data collection and helps maintain organized records.

Automatic Database Update: The scraper keeps track of previously searched URLs to avoid duplication in results. This ensures a more efficient search experience, especially when querying for the same keyword multiple times.

Use Cases
This tool is ideal for researchers, cybersecurity analysts, or anyone interested in exploring dark web resources. It allows users to gather valuable insights from hidden services, facilitating data collection for academic or professional purposes.

Limitations
Access to .onion Domains: Since this tool relies on the Tor network, it can only access .onion websites. Users should be aware of the legal and ethical implications of exploring dark web content.

Rate Limiting: To comply with website policies and avoid overloading servers, the scraper is designed to fetch a limited number of results (up to 20 URLs) per search.

How to Install :-
Installation Instructions
To set up the Tor-Enabled Onion Website Scraper with Keyword Analysis project on your local machine, follow these steps:

Prerequisites
Before installing the project, ensure you have the following:

Python 3.x: Download and install Python from the official website.
Tor: Install the Tor Browser or Tor service. You can download it from torproject.org. Make sure the Tor service is running before executing the scraper.
Step-by-Step Installation
Clone the Repository: Open your terminal or command prompt and run the following command to clone the repository:

bash
git clone https://github.com/your-username/Darkweb-data-Crawler.git
Replace your-username and your-repo-name with your GitHub username and the repository name you created.

Navigate to the Project Directory: Change to the project directory:

bash
cd your-repo-name
Install Required Libraries: Use pip to install the necessary Python libraries. Run the following command:

bash
pip install requests beautifulsoup4 pandas openpyxl
This command installs:

requests: for making HTTP requests.
beautifulsoup4: for parsing HTML content.
pandas: for data manipulation and Excel file handling.
openpyxl: for reading/writing Excel files.
Configure Tor: Ensure that the Tor service is running on your machine. The scraper is configured to use the Tor proxy at localhost:9150. If you have changed the default settings, update the proxy settings in the code accordingly.

Running the Scraper
Execute the Script: After completing the installation, run the scraper using the following command:

bash
python onion_scraper.py
Follow the Prompts:

Enter the keyword you want to search for on .onion websites when prompted.
Provide the output file name (without extension) when asked.
