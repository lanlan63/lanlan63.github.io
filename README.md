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

## Week 2
### Security Planning and Testing Methodology 
Design a security baseline and performance testing methodology.
Deliverables (Journal):
1. Create a performance testing plan describing your remote monitoring methodology and 
testing approach
2. Security Configuration Checklist covering SSH hardening, firewall configuration, mandatory 
access control, automatic updates, user privilege management, and network security
3. Threat Model identifying at least 3 specific security threats with mitigation strategies
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

## Week 7

