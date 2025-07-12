# Advanced Nmap Website Scanner

A powerful web-based network scanner built with Flask that leverages Nmap to perform detailed scans of IP addresses and hostnames. The scanner provides information on open ports, service versions, operating system detection, and more — all through a user-friendly web interface.

---

## Features

- Validates input to accept only valid IPv4 addresses or domain names.
- Runs advanced Nmap scans including SYN scan, version detection, OS detection, and script scanning.
- Displays scan results in a clear format on the web page.
- Allows downloading raw scan results as text files.
- Automatically resolves hostnames to IP addresses.
- Temporary storage of scan reports on the server for easy access.

---

## Requirements

- Python 3.7 or higher
- [Nmap](https://nmap.org/download.html) installed and added to system PATH
- Flask (`pip install Flask`)

---

## Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/advanced-nmap-website-scanner.git
   cd advanced-nmap-website-scanner
   ```
   
    (Optional) Create and activate a virtual environment:
```
python3 -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate
```
Install dependencies:
```
pip install -r requirements.txt
```
Run the Flask application:
```
python main.py
```

Open your browser and visit http://localhost:5000.

Usage

  Enter a valid IP address or hostname on the homepage.

  Click Scan to start the Nmap scan.

  View the detailed scan results on the results page.

  Download the scan report if needed.

Security Notice

  Use responsibly and ensure you have permission to scan target systems.

  Scanning external networks without authorization may be illegal.

  Consider adding authentication and rate limiting before deploying publicly.

Project Structure

  main.py - Main Flask app handling routes and scanning logic.

  templates/ - HTML templates for the UI (index.html, result_real.html).

  Temporary scan results stored in the system temp directory.

