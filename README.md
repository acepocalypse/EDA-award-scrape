# Academic Awards Scraper

This repository contains Python scripts for scraping data from websites of highly prestigious and prestigious academic awards. The goal is to collect information about award recipients, categories, and other relevant details.

## Features

- Scrapes data from multiple academic award websites
- Extracts information such as award names, recipients, categories, and years
- Stores data in a structured format (CSV, JSON, etc.)
- Handles website navigation and pagination
- Includes error handling and logging

## Requirements

- Python 3.8+
- BeautifulSoup4
- Requests
- Pandas
- Selenium (for dynamic content)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/academic-awards-scraper.git
    cd academic-awards-scraper
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Update the `config.json` file with the URLs of the award websites you want to scrape and other configuration details.

2. Run the scraper:
    ```bash
    python scraper.py
    ```

3. The scraped data will be saved in the `output` directory in the specified format.

## Configuration

The `config.json` file should contain the following fields:
- `urls`: List of award website URLs to scrape
- `output_format`: Format to save the scraped data (e.g., CSV, JSON)
- `log_level`: Logging level (e.g., DEBUG, INFO, WARNING)

Example `config.json`:
```json
{
    "urls": [
        "https://example.com/award1",
        "https://example.com/award2"
    ],
    "output_format": "csv",
    "log_level": "INFO"
}
```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgements

- BeautifulSoup4
- Requests
- Pandas
- Selenium