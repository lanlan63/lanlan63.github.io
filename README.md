# Operating Systems Journal - Lani
## Week 1
### System Planning and Distribution Selection
Plan your operating system deployment and justify technical decisions.
Deliverables (for your Journal):
1. Create a System Architecture Diagram showing both systems and network connections
2. Distribution Selection Justification comparing your chosen server distribution with 
alternatives
3. Workstation configuration decision justifying your choice of workstation option
4. Network configuration documentation covering VirtualBox settings and IP addressing
5. Using a CLI, document system specifications using `uname`, `free`, `df -h`, `ip addr`, and 
`lsb_release`
![free and free](https://github.com/user-attachments/assets/103d48af-d61d-4c81-9ad0-f253d0bad065)
![df -h](https://github.com/user-attachments/assets/c20836a5-3563-4ecc-86d9-17424986385e)
![ipadress](https://github.com/user-attachments/assets/3f0ba298-990f-4e67-a7ad-6723999822d3)
![lsbrelease](https://github.com/user-attachments/assets/a5979f32-00d8-4a0b-a3de-ffb3ab99c138)


## Week 2 
### Security Planning and Testing Methodology 
Design a security baseline and performance testing methodology.
Deliverables (Journal):
1. Create a performance testing plan describing your remote monitoring methodology and 
testing approach
2. Security Configuration Checklist covering SSH hardening, firewall configuration, mandatory 
access control, automatic updates, user privilege management, and network security
3. Threat Model identifying at least 3 specific security threats with mitigation strategies

[SS-DONE]
For your journal: Document pipeline examples with explanations. Explain how pipes 
enable process cooperation and data flow between programmes.

For your journal: Screenshots showing named pipe communication. Explain the difference 
between anonymous pipes (|) and named pipes (FIFO), including use cases for each.

For your journal: Signal handling script with explanations. Discuss the importance of 
signal handling in robust applications.

For your journal: Producer/consumer scripts with explanations. Discuss the challenges of 
inter-process synchronisation and race conditions


## Week 3
### Application Selection for Performance Testing 
Select applications representing different workload types for performance evaluation.
Deliverables (Journal):
1. Select applications representing different workload types (e.g. CPU-intensive, RAMintensive, I/O-intensive, Network-intensive, and Server applications such as game servers)
for performance evaluation and create an Application Selection Matrix listing applications 
with justifications for choosing them.
2. Installation Documentation with exact commands for SSH-based installation
3. Expected Resource Profiles documenting anticipated resource usage
4. Monitoring Strategy explaining measurement approach for each application

For your journal: Take screenshots showing process listings with visible command 
prompts. Explain what the different process states (R, S, D, Z, T) represent.

For your journal: Document the process lifecycle with examples. Explain when you would 
use foreground vs background processes, and the difference between kill and kill -9.

To get ssh to work on ubuntu I had to install it first using:
sudo apt-get install openssh-server
as it is not automatically installed 

For your journal: Take a screenshot showing key generation. Explain why ed25519 is 
recommended over RSA for new keys.
For your journal: Screenshot showing successful passwordless SSH connection with 
visible command prompt showing username@hostname on both systems.
For your journal: Include before and after screenshots of the sshd_config file showing the 
critical security changes. Explain why each setting improves security.
For your journal: Document your complete firewall ruleset with screenshots. Create a 
table showing each rule, its purpose, and security justification.
For your journal: Document the user creation process with screenshots. Explain the 
principle of least privilege and why using a non-root administrative user is important.
For your journal: Screenshots demonstrating that all server administration is performed 
via SSH from the workstation, not from the server console.

initial secuity pdf (WEEK7 LAB)

## Week 4
### Initial System Configuration & Security Implementation 
Deploy your server and implement foundational security controls.
Deliverables (Journal and Video):
1. Configure SSH with key-based authentication
2. Configure a firewall permitting SSH from one specific workstation only
3. Manage users and implement privilege management, creating a non-root administrative 
user.
4. SSH Access Evidence showing successful connection screenshots
5. Configuration Files with before and after comparisons
6. Firewall Documentation showing complete ruleset
7. Remote Administration Evidence demonstrating commands executed via SSH
Administrative Constraint: All server configurations must be performed via SSH from your 
workstation.

week8 lab activity pdf

## Week 5
### Advanced Security and Monitoring Infrastructure 
Implement advanced security controls and develop monitoring capabilities.
Deliverables (Journal and Video):
1. Implement Access Control using SELinux or AppArmor, with documentation showing how to 
track and report on access control settings.
2. Configure automatic security updates with evidence of implementation
3. Configure fail2ban for enhanced intrusion detection
4. Create a security baseline verification script (`security-baseline.sh`) that runs on the server
(executed via SSH) and verifies all security configurations from Phases 4 and 5.
5. Create a remote monitoring script (`monitor-server.sh`) that runs on your workstation, 
connects via SSH, and collects performance metrics from the server.
Note:
All scripts should include line-by-line comments explaining their functionality. All 
implementations must be demonstrated in your video with live command execution and 
explanation.

## Week 6
Phase 6: Performance Evaluation and Analysis (Week 6)
Execute detailed performance testing and analyse operating system behaviour under different 
workloads.
Testing Methodology:
For each application or service, you have chosen, select, monitor and compare the following, 
where appropriate:
1. CPU usage
2. Memory usage
3. Disk I/O performance
4. Network performance
5. System latency
6. Service response times.
Testing Scenarios:
For each application or service, you have chosen, select, monitor and compare the following, 
where appropriate:
• Baseline performance testing
• Application load testing
• Performance analysis identifying bottlenecks
• Optimisation testing. Aim to implement and evidence at least two improvements.
Deliverables (Journal and Video):
1. Document your approach
2. Create a performance data table with structured measurements for all applications and 
metrics
3. Create performance visualisations including charts and graphs
4. Capture testing evidence
5. Conduct network performance analysis documenting latency and throughput
6. Capture optimisation analysis results describing improvements with quantitative data

## Week 7
Phase 7: Security Audit and System Evaluation (Week 7)
Conduct a security audit and evaluate overall system configuration.
Mandatory Audit Tasks: Security scanning with Lynis, network security assessment with 
nmap, access control verification, service audit justifying all running services, and system 
configuration review.
Deliverables (Journal and Video):
1. Security Audit Report covering infrastructure security assessment, Lynis scores before and 
after remediation, network security testing results, SSH security verification, service 
inventory with justifications, and remaining risk assessment
