# PortScanner
A simple multi-threaded port scanner written in Python. PortScanner accepts one or multiple targets (IP addresses or hostnames) and a port range to scan. It attempts to connect to each port and prints whether the port is open and service banner when possible.
## ⚠️ Important
Use responsibly

This tool is intended for educational purposes, network debugging, and authorized security testing only. Do not scan networks, hosts, or services you do not own or do not have explicit permission to test. Unauthorized scanning can be considered illegal or hostile activity in many jurisdictions.

# Features
1. Scan a single target or multiple targets (comma-separated).

2. Scan a range of ports or the full TCP port space.

3. Attempts to read a service banner when a connection is successful.

4. Simple multi-threaded design to perform scans concurrently.

# Requirements
Operating System : Linux , Windows , MacOS

Dependencies : python3 , IPy library

Install dependencies with pip:
```
pip install IPy
```




