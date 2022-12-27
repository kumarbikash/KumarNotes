# Areas for Server Security

## System Patching
- AIX - NIM Server
- Linux - SuSE Manager/ YaST/ Zypper
- Windows - WSUS/ MBSA/ VAPT scanner

## Antivirus
Updated one and on all nodes in the network, with relevant policies

## System Monitoring
- Centreon/ Nagios
Regular and scheduled scanning of the entire network 

## Anonymous Shares
No anonymous shares, OR limited to a bare minimum if can't 

## Operating System Version 
Always latest and approved
Discard or avoid EOL listed versions/ editions

## Remote Access
RDP/ SSH
iLO/ iDRAC/ RSA/ iRMC/ vSphere/ vCenter
No VNC etc.

## Standard Installation
-Restricted or Controlled access to Installation sources
-Regular update/ patching of the Installation sources
-The created passwords within the Installation scripts should not be accessible immediately after the shortest possible context
-Vulnerability scan should be among the last steps to be executed for each installation

Using:
- Windows - System Center Configuration Manager (SCCM)
- Linux - SCCM/ AutoYast
- vSphere
- AIX - NIM Server

## Server Hardening
ASLR (Address Space Layout Randomization)

- Limit the open ports and applications to absolute minimum (reduce the surface)
- Domain accounts instead of local accounts
- Host based firewall
- Whitelisting

## Protect Local Admin accounts
Ensure local Administrator account is disabled
Do not use built-in administrator accounts as service accounts or to log in (except for Disaster Recovery scenarios without domain access)

## Logging
Syslog

Log should contain:
- Logged event
- Date and time
- User and/ or process associated
- Any additional information

Logs should be kpet centrally for 90-180 days at a minimum
For any post incident analysis to work properly, ensure that all the machines have their times synced with NTP servers

- /var/log/messages | /var/log/audit
- logfile compression and rotation should be used

## Storage Device Cleaning
- Industry grade data erasing before reuse on another system within company
- Industry grade data wiping or destroying physically before discarding/ disposing/ returning to OEM etc.

## Physical Security
Physical security measures for access to servers

## Access Management
User access to servers, should be well-controlled
Encourage to use four-eye-principle while granting any access to servers

## Administration and System Accounts
- Avoid connecting remotely using built-in Administrative/ System accounts
- Using management tools like iLO etc., the built-in Administrative accounts may be used
- Password change every 90 days minimum with recommended complexity and length
- Disable/ delete accounts which are not in use

## No network bridge via the server
- The network zones which are separated by firewalls, should not be bridged via any of the servers, i.e. no servers should have direct connection with multiple network zones

## Appliances
- Any appliance where company standard OS has not been installed, should be rated as "untrusted"
- The hardening steps mentioned in this document should be applied to such appliances, wherever feasible
- Detailed review of the appliance should be done from security risk angle like vendor user accounts, remote access, scheduled automated tasks, unwanted open port, known vulnerabilities, etc.
- Regular scan of the appliance for ensuring security risk posture and compliance

## NTLMv2 or Kerberos
- Use NTLMv2 or Kerberos instead of LM and NTLM authentication (better to go for Kerberos wherever feasible)

## Automatic Session Lock
After period of inactivity (say 15 minutes), user session should be locked

## Tier model
To avoid elevation of privileges, accounts should be mapped to one tier at any time
- DMZ Tier (DMZ admins)
- DC Tier (Forest admins)
- Server Tier (Server admins)
- Workstation Tier (Workstation admins and users)

MFA is recommended to protect admin accounts

