# Advanced Nmap Website Scanner
[Official Demo Website](https://c01378ea-e2ef-49fc-a5ea-189adcdf11a0-00-21gdtq58c01lg.riker.replit.dev/) 

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
## Screenshots

![Screenshot 2025-07-12 060930](https://github.com/user-attachments/assets/04acfe30-fc8f-4cfb-8611-622fbc6e50aa)

![Screenshot 2025-07-12 060900](https://github.com/user-attachments/assets/d1d959d4-bfe0-4b10-a3a4-cd98e9f157cf)

![Screenshot 2025-07-12 060955](https://github.com/user-attachments/assets/a70c7116-0f17-4d15-a9ad-3269b3022db1)

## Requirements

- Python 3.7 or higher
- [Nmap](https://nmap.org/download.html) installed and added to system PATH
- Flask
  
  ```bash
  pip install Flask
  ```

---

## Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yossefibrahimmohamed/Nmap_Scanner_Advanced.git
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

  Please take a look at the detailed scan results on the results page.

  Download the scan report if needed.

Security Notice

  Use responsibly and ensure you have permission to scan target systems.

  Scanning external networks without authorization may be illegal.

  Consider adding authentication and rate limiting before deploying publicly.

Project Structure

  main.py - Main Flask app handling routes and scanning logic.

  templates/ - HTML templates for the UI (index.html, result_real.html).

  Temporary scan results stored in the system temp directory.

