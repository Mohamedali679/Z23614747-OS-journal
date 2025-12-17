Week 7 – Security Audit and Final Evaluation

This week focuses on reviewing the system after all configuration, security, and testing work has been completed. The aim is to check the overall security state of the server and evaluate whether the system meets the original goals of the coursework.

Security audit overview

A basic security audit was carried out to review the current state of the server. This involved checking user accounts, running services, firewall rules, and security tools that were enabled during previous weeks.

The audit helped identify whether any unnecessary services were running and whether security controls were correctly applied.

Service and port review

The list of running services was reviewed to ensure that only required services were active. Any services that were not needed for the server’s purpose were disabled.

Network ports were also checked to confirm that only SSH was accessible externally. This helped reduce the attack surface of the system.

Security tools verification

Security tools such as the firewall, AppArmor, and fail2ban were checked to confirm that they were active and running as expected.

These tools provided multiple layers of protection, including network filtering, access control, and protection against repeated login attempts.

Audit findings

The audit showed that the server was reasonably secure for its intended purpose. Remote access was restricted, unnecessary services were removed, and security controls were in place.

No critical security issues were identified during the audit. Any minor configuration improvements could be addressed in future updates.

Final evaluation

Overall, the system met the goals set at the beginning of the project. The server was successfully deployed, secured, and tested using command line tools and remote administration.

The coursework demonstrated how operating system features such as user management, access control, networking, and process management work together in a real server environment.

Reflection

This project helped improve my understanding of Linux system administration and operating system concepts. Planning the system first made implementation easier and reduced mistakes.

Working with a headless server and managing it remotely showed how real servers are operated in practice. The combination of security, performance testing, and auditing helped reinforce how important operating system configuration is for building reliable systems.
