# CSC 3570 – IT Security

**Lab 1:**

  Windows 10 Workstation
    - Updated Windows 10 operating system.
    - Added a new administrative account for the team.
    - Set static IP: 192.168.1.122 with subnet mask 255.255.255.128, gateway 192.168.1.121, and DNS 192.168.1.121.

  OpenWrt Router
    - Set initial password for router access.
    - Added DMZ port to DNS server: Enabled under Network → DHCP and DNS → Devices & Ports → Listen Interfaces → DMZ.

  Windows Server 2019
    - Verified administrative access using provided credentials.
    - Forced password requirement for Administrator account.
    - Set static IP: 192.168.1.121 with subnet mask 255.255.255.128, gateway 192.168.1.1, and DNS 192.168.1.1.
    - Installed Active Directory Domain Services and DNS Server roles.
    - Promoted server to Domain Controller for new forest `pompeii13.net`.
    - Configured Directory Services Restore Mode (DSRM) password.
    - Added Windows 10 workstation to domain `pompeii13.net` and updated workstation DNS to point to domain controller.
    - Verified login to domain using domain credentials.
    - Applied all available Windows Server updates.

  Ubuntu Server
    - Created new user accounts with `sudo` privileges.
    - Updated system packages (without performing a dist-upgrade).
    - Installed Apache2 and PHP.

  General Security / Lab Principles Applied
    - Ensured separation of domains and duties.
    - Maintained isolation and encapsulation of systems.
    - Applied modularity and simple design principles.
    - Followed least privilege and fail-safe defaults where applicable.
    - Minimized trust surface and enforced complete mediation.
    - Documented all changes and actions systematically for team reference.
