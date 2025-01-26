# Automated-Port-Scanner
A lightweight port scanner using netcat or nmap to identify open ports on a given host and flag vulnerable services.



How to Use:
Install required tools (if not installed):


sudo apt install nmap netcat
Save the script:
Save the script as port_scanner.sh.

Make the script executable:


----------------------------

chmod +x port_scanner.sh
Run the script:
--------------------------


---------------------------------
./port_scanner.sh
-----------------------------


Features:
Interactive Command-Line Interface:

User-friendly prompts to enter the target host and port range.
Option to choose between nmap (detailed scan) and netcat (quick scan).
Scan Methods:

Nmap Scan: Performs service detection and reports open ports.
Netcat Scan: Performs basic TCP checks for open ports.
Port Range Selection:

Users can define a custom port range (e.g., 1-65535) or use the default common ports.
Vulnerability Detection:

Checks for commonly vulnerable services such as FTP, SSH, HTTP, etc.
Logging:

Logs scan results in port_scan.log for future reference.

---------------------------
Automation (Optional):

You can automate the script by adding it to a cron job:

crontab -e
Example to run the script every night at midnight:

0 0 * * * /path/to/port_scanner.sh
