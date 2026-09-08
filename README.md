# Nmap Network Scanning Lab

## Objective

To learn how Nmap can be used to identify open ports and running services on a controlled local laboratory system.

## Lab Environment

- Operating System: Kali Linux
- Virtualization: VirtualBox
- Scanning Tool: Nmap
- Target: Localhost (127.0.0.1)
- Web Server: Python SimpleHTTPServer

## Methodology

1. Performed a basic Nmap scan against localhost.
2. Started a Python HTTP server on TCP port 8000.
3. Scanned localhost again to identify the newly available port.
4. Used Nmap service/version detection to identify the service.
5. Saved the scan results for documentation.

## Results

The initial scan identified no open ports among Nmap's default 1,000 TCP ports.

After starting the Python HTTP server, TCP port 8000 was detected as open.

Service/version detection identified:

8000/tcp - HTTP - SimpleHTTPServer 0.6 (Python 3.13.12)

## Security Analysis

An open port indicates that a service is accepting network connections.

In a real environment, unnecessary services should be disabled or properly secured because exposed services can increase the attack surface.

This experiment was performed only on a controlled local laboratory system.

## Skills Demonstrated

- Linux command line
- Network scanning
- Nmap
- Port identification
- Service enumeration
- Basic security analysis
- Technical documentation
