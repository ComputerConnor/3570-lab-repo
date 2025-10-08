# CSC 3570 – IT Security

**Lab 1:**

  Windows 10 Workstation <br>
    - Updated Windows 10 operating system.<br>
    - Added a new administrative account for the team.<br>
    - Set static IP: 192.168.1.122 with subnet mask 255.255.255.128, gateway 192.168.1.121, and DNS 192.168.1.121.<br>

  OpenWrt Router <br>
    - Set initial password for router access.<br>
    - Added DMZ port to DNS server<br>

  Windows Server 2019 <br>
    - Verified administrative access using provided credentials.<br>
    - Forced password requirement for Administrator account.<br>
    - Set static IP: 192.168.1.121 with subnet mask 255.255.255.128, gateway 192.168.1.1, and DNS 192.168.1.1.<br>
    - Installed Active Directory Domain Services and DNS Server roles.<br>
    - Promoted server to Domain Controller for new forest `pompeii13.net`.<br>
    - Configured Directory Services Restore Mode password.<br>
    - Added Windows 10 workstation to domain `pompeii13.net` and updated workstation DNS to point to domain controller.<br>
    - Verified login to domain using domain credentials.<br>
    - Applied all available Windows Server updates.<br>

  Ubuntu Server <br>
    - Created new user accounts with `sudo` privileges.<br>
    - Updated system packages (without performing a dist-upgrade).<br>
    - Installed Apache2 and PHP.<br>

---------------------------------------------------------------------------------------------------------------------------------------------------- <br>

**Lab 2:**

  Windows 10 Workstation
    - Installed Malwarebytes Free and ran a quick scan.<br>

  Windows Server
    - Added user `devops` to Active Directory with password `Password123!`.<br>
    - Assigned `devops` user to Domain Admins group.<br>
    - Installed Malwarebytes Free and ran a quick scan.<br>

  WWW Server (Ubuntu)
    - Created `devops` user and added to sudo group with password `Password123!`.<br>
    - Installed ClamAV and ran a scan on `/usr/local/bin/` recursively using `-r` and `-i` flags.<br>
    - Installed Lynis and ran system audit using `lynis audit system --quick`.<br>
    - Analyzed top suggestions from Lynis log (`/var/log/lynis.log`).<br>

  Jumpboxes (Ubuntu)
    - Installed dependencies for Flan Scan: curl, git, make, docker.io, firefox.<br>
    - Installed and ran Flan Scan following guide from Cloudflare.<br>
    - Scanned Windows Server at `192.168.1.121`.<br>
    - Scanned Branch Office Linux server at `10.0.14.4`.<br>
    - Saved HTML reports in `shared/reports/` directory.<br>

  
