Week 5 – Advanced Security and Basic Automation

This week focuses on adding more security controls to the server and introducing basic automation. The aim is to improve protection while also reducing the amount of manual work needed to check the system.

AppArmor configuration

Ubuntu Server uses AppArmor to control what applications are allowed to do on the system. AppArmor profiles limit access to files, system resources, and capabilities.

During this week, I checked which AppArmor profiles were already enabled on the system. I also ensured that AppArmor was active and enforcing rules. This adds an extra layer of security in case an application is compromised.

The use of AppArmor helps reduce damage by limiting what processes can access, even if they are exploited.

Fail2ban setup

Fail2ban was installed and configured to protect the SSH service. Its purpose is to detect repeated failed login attempts and temporarily block the source address.

This helps protect the server from brute force attacks against SSH. Once enabled, fail2ban runs automatically in the background and does not require manual monitoring.

Basic automation scripts

To reduce repetitive tasks, simple automation scripts were introduced. These scripts are written in bash and are used to collect basic system information.

Examples of tasks automated include checking disk usage, memory usage, and system uptime. Automating these checks makes it easier to monitor the system consistently.

The scripts are stored in a scripts folder and can be run manually or scheduled to run at specific times.

Security and automation benefits

Using automation reduces the chance of human error and saves time. It also ensures system checks are performed in a consistent way.

Combining automation with security tools like AppArmor and fail2ban creates a more reliable and secure system without adding too much complexity.

Reflection

This week showed how security can be strengthened beyond basic settings. Adding AppArmor and fail2ban made the system more resistant to common attacks.

Writing simple scripts also helped me understand how automation can support system administration tasks and make monitoring easier.
