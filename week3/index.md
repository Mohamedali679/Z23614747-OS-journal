Week 3 – Application Selection for Performance Testing

This week focuses on choosing applications that will be used later to test system performance. The idea is to use different types of workloads so that CPU, memory, disk, and network behaviour can be observed.

The applications selected are not meant to be complex. They are chosen because they represent common workload types and are easy to install and test on a server system.

Application selection

To cover different workload types, I selected the following applications and tools.

CPU intensive workload  
For CPU testing, I will use a stress testing tool that can create high CPU usage. This will help show how the operating system schedules processes and handles high processor load.

Memory intensive workload  
For memory testing, I will use a tool that allocates large amounts of RAM. This will allow me to observe memory usage, caching, and how the system behaves when memory pressure increases.

Disk and I O workload  
For disk testing, I will use basic file operations such as writing and reading large files. This will show disk usage, disk speed, and how I O operations affect overall system performance.

Network intensive workload  
For network testing, I will use a simple network testing tool to send data between the workstation and the server. This will help measure network throughput and latency over the virtual network.

Server type workload  
To represent a real server application, I plan to use a lightweight service such as a simple web service. This will allow me to observe background service behaviour and response times.

Application selection summary

The chosen applications represent a mix of CPU heavy, memory heavy, disk heavy, and network heavy workloads. Together, they provide a good range of scenarios to test how the operating system performs under different conditions.

Installation approach

All applications will be installed on the server using the command line over SSH. Package installation will be done using the system package manager. This follows the coursework requirement of using SSH for all administration tasks.

Exact installation commands will be recorded later once the server is fully configured and secured.

Expected resource usage

Before testing, I expect the following behaviour.

CPU tests will mainly increase processor usage with minimal impact on disk and network.  
Memory tests will increase RAM usage and may affect system responsiveness.  
Disk tests will increase disk activity and I O wait time.  
Network tests will increase network traffic between the workstation and the server.  
Server applications will use moderate resources continuously while running.

Monitoring strategy

System monitoring will be done remotely using command line tools over SSH. These tools will be used to observe CPU usage, memory usage, disk activity, and network usage while each workload is running.

Baseline measurements will be taken before starting any workload. Measurements during testing will then be compared with the baseline to identify performance changes and bottlenecks.

Reflection

This week helped me understand that different applications stress different parts of the operating system. Choosing a mix of workloads makes performance testing more meaningful.

Planning the applications in advance also makes it easier to design monitoring and testing methods for later weeks, rather than choosing tools randomly during testing.
