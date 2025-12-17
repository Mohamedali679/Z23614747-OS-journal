Week 6 – Performance Testing and System Behaviour

This week focuses on testing system performance and observing how the operating system behaves under different workloads. The aim is to understand how CPU, memory, disk, and network usage change when the server is under load.

Baseline performance

Before running any workloads, baseline measurements were taken while the system was mostly idle. This helped establish what normal resource usage looks like without stress.

Baseline checks showed low CPU usage, stable memory usage, minimal disk activity, and low network traffic. These results were used as a reference point for later testing.

CPU performance testing

A CPU intensive workload was run to increase processor usage. During this test, CPU usage increased significantly while memory and disk usage stayed relatively low.

This showed how the operating system schedules processes and handles high processor demand. The system remained responsive, but CPU usage stayed high while the workload was running.

Memory performance testing

A memory intensive workload was used to increase RAM usage. During this test, memory usage increased steadily, and cached memory also changed.

The system handled the increased memory usage without crashing. This helped demonstrate how the operating system manages available memory and caching.

Disk performance testing

Disk testing was carried out by reading and writing large files. During this test, disk activity increased and input output operations became more frequent.

This showed how disk usage affects system performance and how file operations contribute to overall load.

Network performance testing

Network testing was performed between the workstation and the server over the virtual network. During this test, network traffic increased and data transfer could be observed.

This helped show how the network behaves under load and how virtual networking affects performance.

Security impact on performance

Security features such as the firewall, AppArmor, and fail2ban were enabled during testing. These features did not cause major performance issues during the tests.

Any performance impact from security controls appeared to be small compared to the workload itself.

Reflection

This week helped me understand how different workloads affect different system resources. CPU heavy tasks mainly affect processor usage, while memory, disk, and network tests stress other parts of the system.

Comparing baseline measurements with workload results made it easier to see how the operating system responds to increased demand. This understanding will be useful when evaluating the system in the final audit.
