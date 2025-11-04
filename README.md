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


# Setup Instructions
1. Clone the repository to your local machine:
```
git clone https://github.com/kr-anish/PortScanner
```
2. Install dependencies:
```
pip install -r requirements.txt
```
3. Run the script from the command line.
```
python3 PortScanner.py
```

# Usage
Run the script from the command line. The script prompts for targets and a port range.
```
python3 PortScanner.py
```
Enter the target to scan and the port range
<img width="1912" height="918" alt="Image" src="https://github.com/user-attachments/assets/a6ca4d0d-e223-4610-b2c6-2e9d164c4dc2" />

Note:

• If you press Enter without - in the port prompt, the script will default to scanning all TCP ports (1-65535).

• When providing multiple targets, separate them with commas.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/61952b48-a93a-44c0-82c3-3ca545051253" />

# Troubleshooting
• ModuleNotFoundError: No module named 'IPy' —> Install the IPy package: pip install IPy.

• socket.gaierror when resolving hostnames —> check your DNS or the hostname spelling.

• If scanning localhost or very large port ranges, you may hit system limits for threads or open file descriptors. Use a thread pool or reduce the range.


