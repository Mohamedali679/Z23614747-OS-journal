Week 2 – Security Planning and Testing

This week is focused on planning how the server will be secured and how performance will be tested later on. Before changing any settings on the server, it is important to think about possible security risks and how they can be reduced.

Performance testing plan

Before running applications on the server, I need a clear idea of how performance will be measured. The main aim is to understand how the operating system behaves under different workloads.

The areas I plan to monitor are CPU usage, memory usage, disk usage, and network usage.

I will first record baseline performance when the system is mostly idle. Later, I will compare this with results collected while applications are running. All monitoring will be done remotely from my workstation using SSH.

Security planning checklist

To keep the server secure, I created a list of security steps that will be applied over the next few weeks.

These steps include securing SSH access, disabling root login, using SSH keys instead of passwords, configuring a firewall to only allow SSH from my laptop, creating a normal user account, enabling automatic security updates, using AppArmor for access control, installing fail2ban to reduce login attacks, and disabling unnecessary services.

This checklist helps make sure security is applied in an organised way and nothing important is missed.

Threat model

A threat model helps identify what could go wrong and how the risk can be reduced.

The first threat is unauthorised SSH access. If SSH is not secured, someone could try to guess passwords or gain access to the server. This risk will be reduced by using SSH keys, disabling password login, limiting SSH access with firewall rules, and blocking repeated failed login attempts.

The second threat is having too much privilege. If everything is done as root, any mistake or security issue could affect the entire system. This will be reduced by using a normal user account and only using sudo when it is needed.

The third threat is unnecessary services running on the server. Services that are not required can increase security risks. This will be reduced by checking which services are running, disabling ones that are not needed, and justifying all remaining services later in the audit.

Security and performance

Some security features can slightly affect system performance. Logging, access control, and intrusion protection can use extra system resources. At this stage, the impact is expected to be small, but later performance tests will show whether security settings have any noticeable effect.

Reflection

This week showed that security needs to be planned before making changes to the system. Writing down possible risks made it easier to understand what needs to be protected. It also helped me think about how security decisions might affect performance in later stages of the coursework.
