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
<img width="411" height="91" alt="Screenshot 2025-11-28 151826" src="https://github.com/user-attachments/assets/bc0022d3-e3b3-410d-9c65-3938ba38fc38" />

<img width="416" height="157" alt="Screenshot 2025-11-28 152746" src="https://github.com/user-attachments/assets/103d48af-d61d-4c81-9ad0-f253d0bad065" />
<img width="421" height="214" alt="Screenshot 2025-11-28 152817" src="https://github.com/user-attachments/assets/c20836a5-3563-4ecc-86d9-17424986385e" />
<img width="421" height="38" alt="Screenshot 2025-11-28 152914" src="https://github.com/user-attachments/assets/3f0ba298-990f-4e67-a7ad-6723999822d3" />
<img width="439" height="50" alt="Screenshot 2025-11-28 153414" src="https://github.com/user-attachments/assets/a5979f32-00d8-4a0b-a3de-ffb3ab99c138" />


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

