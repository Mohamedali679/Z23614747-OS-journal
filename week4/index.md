Week 4 – Initial System Configuration and Security Implementation

This week focuses on setting up the server properly and applying the first security controls. All configuration was done remotely from the workstation using SSH, as required by the coursework.

Server access and SSH setup

After installing Ubuntu Server, I connected to the system remotely using SSH from my Windows laptop. This confirmed that remote administration was working correctly.

SSH access was configured to use key based authentication instead of passwords. This improves security by reducing the risk of brute force attacks. Password based login was disabled after confirming that key access was working.

The SSH configuration file was edited to apply these changes and the SSH service was restarted to activate them.

User and privilege management

A new non root user account was created for normal administration tasks. This user was added to the sudo group so administrative commands could still be run when needed.

Using a normal user instead of logging in as root reduces the risk of accidental system changes and limits the impact if an account is compromised.

Firewall configuration

A firewall was enabled on the server to control incoming network traffic. The firewall rules were configured to allow SSH connections only from the workstation over the host only network.

All other incoming connections were blocked by default. This reduces the attack surface of the server and ensures only authorised access is allowed.

Remote administration confirmation

All configuration tasks were performed remotely using SSH. Commands were executed from the workstation and changes were applied on the server without using a graphical interface or direct console access.

Successful SSH connections and command execution confirmed that remote administration was functioning as expected.

Configuration evidence

Before and after changes were checked by reviewing configuration files and service status. This helped confirm that the security settings were applied correctly and that no services were accidentally broken.

Reflection

This week helped me understand the importance of basic security configuration before running applications or performance tests. Setting up SSH keys, user accounts, and firewall rules created a more secure base system.

Working entirely through SSH also reinforced command line skills and showed how remote server administration works in practice.
