# ShodanPortInspector

ShodanPortInspector is a Python-based OSINT learning project that uses the Shodan API to collect publicly available information about internet-facing systems. The tool accepts a public IPv4 address or a domain name, resolves domains to IP addresses using DNS, and retrieves indexed data such as open ports, organization details, and operating system information.

The project includes a basic risk check that flags commonly exposed ports such as FTP (21), SSH (22), Telnet (23), MySQL (3306), and RDP (3389). This analysis is intentionally simple and focuses on understanding exposure rather than performing vulnerability scanning or exploitation.

ShodanPortInspector does not perform active network scanning and does not work on private IP addresses or IPv6 addresses. All data is sourced from Shodan’s existing database, and results depend on what Shodan has already indexed.

Scan results are displayed on the console and saved locally with a timestamp for reference. Error handling is implemented to manage invalid inputs, unavailable Shodan data, and API-related issues without crashing the program.

## Features
- Accepts public IPv4 addresses or domain names
- Resolves domains to IP addresses using DNS
- Fetches publicly indexed data from the Shodan API
- Displays open ports, organization, and OS information
- Flags commonly risky ports
- Saves scan results locally with timestamps

## Technologies Used
- Python
- Shodan API
- Socket library
- Environment variables

## How to Run
1. Install the required dependency:
   pip install shodan
2. Set your Shodan API key as an environment variable:
   SHODAN_API_KEY
3. Run the Python script
4. Enter a domain name or public IP address when prompted

## Limitations
- Works only with public IPv4 addresses
- Does not support private IPs or IPv6
- Does not perform live scanning or exploitation
- Output depends on Shodan’s indexed data

## Learning Outcome
This project helped in understanding Python API integration, client–server communication, DNS resolution, basic OSINT reconnaissance, and safe error handling practices.


