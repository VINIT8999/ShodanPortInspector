ShodanPortInspector
Project Overview

ShodanPortInspector is a Python-based reconnaissance tool created as a learning project to understand how publicly available internet data can be accessed using the Shodan API. The project focuses on gathering basic information about public IP addresses or domains without performing any active scanning or exploitation.

This tool helps in understanding how exposed services and open ports can be identified using OSINT (Open Source Intelligence) techniques.

What This Project Does

Accepts a public IPv4 address or domain name as input

Converts domain names into IP addresses using DNS resolution

Fetches publicly indexed data from Shodan

Displays open ports, organization name, and operating system (if available)

Flags commonly risky ports such as FTP, SSH, Telnet, MySQL, and RDP

Saves scan results locally with a timestamp

What This Project Does NOT Do

It does not scan networks directly

It does not work on private IP addresses

It does not exploit vulnerabilities

It does not bypass security controls

This project only uses existing Shodan data.

Technologies Used

Python

Shodan API

Socket (DNS resolution)

OS environment variables

How to Run

Install the Shodan library

pip install shodan


Set your Shodan API key as an environment variable

Run the Python file

Enter a domain or public IP when prompted

Learning Outcome

This project helped me understand:

Client–server communication

API integration in Python

DNS resolution

Basic reconnaissance concepts

Safe handling of errors and inputs
