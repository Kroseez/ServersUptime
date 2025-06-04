# ServersUptime
Script that collects Uptime statistics from all Windows servers using AD and PowerShell
The task at hand was of a technical nature:
The creation of a file containing uptime statistics for all servers was accomplished, and a rudimentary script was formulated to execute the task in its entirety.
The function of the script is as follows:
1. The script performs a check to determine whether a directory exists on the user's disc, specifically the C:\Logs\Uptime directory. In the event that the directory is not present, the script will initiate the creation of the directory.
2. The script is compatible with RSAT. In order to execute the script, it is necessary to have a device with the RSAT package fully installed and an Active Directory administrative account.
3. The script utilises AD to access a pre-coded OU where the servers are located, and it accesses each server by DNS name, performing several actions.
The protocol is designed to verify the status of the server, determining whether it is currently operational or not.
In the event of the server being online, the script will initiate a connection and proceed to collect uptime statistics.
4. Upon completion of the script, a CSV file is generated containing a comprehensive inventory of servers, their online/offline status, and the uptime statistics for online servers.
