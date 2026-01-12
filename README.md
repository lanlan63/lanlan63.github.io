# Operating Systems Journal 
Project overview:
This journal documents 7 weeks of coursework centered around the implementation of my chosen linuz distrobution (Ubuntu) and what I did to configure, and enhance its security alongside evaluating its performance. 

Table of contents:
[Week 1](#week-1)
[Week 2](#week-2)
[Week 3](#week-3)
[Week 4](#week-4)
[Week 5](#week-5)
[Week 6](#week-6)
[Week 7](#week-7)



## Week 1
### System Planning and Distribution Selection
Between Ubuntu and Arch Linux, I decided to use Ubuntu because I was more familiar with it.
Both distros use a monolithic type kernal which means you can modify and interact a lot more with the computer, as things such as process managment and IPC is easily acccesable through the kernal.  
![archdia](https://github.com/user-attachments/assets/04b96675-4da5-4b55-b773-795553eb287c)

Ubuntu is very beginner friendly as it doesnt require a lot of set up to get it working and a good majority of tasks can be done simply with the GUI, while still alllowing free range to do it through the kernal as well, making it good to practice on. Arch LInux requires a lot more CLI use and research with file editing to get it set up and working, but its better for a wider range of customisation options and configuration of your system.
I used oracle VirtualBox in order to run Ubuntu within a virtual machine. 
Here I used the command line interface to find out more information about the current system I was using using different commands.
![free and free](https://github.com/user-attachments/assets/103d48af-d61d-4c81-9ad0-f253d0bad065)
> [!NOTE]
> Uname tells me information about the linux systems I am using with the -a option to display anthing available, df gives me details about the disk space with the -h option to put it in a human readable format, free displays all used and available memory,

![df -h](https://github.com/user-attachments/assets/c20836a5-3563-4ecc-86d9-17424986385e)
> [!NOTE]
> ip is a networking command and the adrr options lets me see the ip adress for my computer.

![ipadress](https://github.com/user-attachments/assets/3f0ba298-990f-4e67-a7ad-6723999822d3)
> [!NOTE]
> hostname shows my domain name system and with the i- options also lets me see my ip adress

![lsbrelease](https://github.com/user-attachments/assets/a5979f32-00d8-4a0b-a3de-ffb3ab99c138)
> [!NOTE]
> lsb_release displays the distro information


## Week 2 
### Security Planning and Testing Methodology 
Performance testing plan:  
Load - I want to simulates a real-world load on the distro to see how it performs under stress.  
Stress - I want to test the distros ability to handle a high load above normal usage levels.  
Endurance - I want to observe the distros behaviour under a large load over a long period.  

Security configuration:\
- [x] SSH hardening
- [x] Firewall configuration
- [x] Mandatory access control
- [x] Turn on automatic updates
- [x] Manage user privalege
- [ ] Network security

Threat modeling:\
1. Someone pretending to be ssomething else - Mitigation stargetgie =Firewall, SSH hardening
2. Altering data or stealing private files - User privaledge, mandatory acess control
3 Malware - Automatic updates, install malware detector


For your journal: Document pipeline examples with explanations. Explain how pipes 
enable process cooperation and data flow between programmes.

For your journal: Screenshots showing named pipe communication. Explain the difference 
between anonymous pipes (|) and named pipes (FIFO), including use cases for each.

For your journal: Signal handling script with explanations. Discuss the importance of 
signal handling in robust applications.

For your journal: Producer/consumer scripts with explanations. Discuss the challenges of 
inter-process synchronisation and race conditions
![df -h](https://github.com/user-attachments/assets/aca97e9e-22f1-4976-8b1c-c4d356ba26b3)
![df -h](https://github.com/user-attachments/assets/d9177941-3a81-47fa-a3ba-502763fa85ac)
![df -h](https://github.com/user-attachments/assets/07809b92-b852-42d7-a6ff-7a807c700dd4)
![df -h](https://github.com/user-attachments/assets/4394535e-769d-403c-89b1-2ff86d7974c9)
![df -h](https://github.com/user-attachments/assets/2497ea41-1a8b-4d8a-93dd-6993f6f74ee6)
![df -h](https://github.com/user-attachments/assets/37c54520-14d6-4fc2-be8a-97612ff39f72)
![df -h](https://github.com/user-attachments/assets/2fb3a7cc-81d1-43a7-b738-8c35fa2f7a18)
![df -h](https://github.com/user-attachments/assets/2075a7a5-1d98-47b9-8b75-fd2a1141f5ee)
![df -h](https://github.com/user-attachments/assets/7d2dc477-fb33-4f80-85f0-fd4006ab5b2c)
![df -h](https://github.com/user-attachments/assets/89f37fee-27b9-4372-9741-99f728de1124)
![df -h]("https://github.com/user-attachments/assets/10b0eb67-3bba-4188-a891-caa927320c64)
![df -h](https://github.com/user-attachments/assets/3607739d-50d6-4d00-adaf-6ac6882f82a4)
![df -h](https://github.com/user-attachments/assets/230417d1-6781-4bb2-bc99-72a1c0bf84c8)
![df -h](https://github.com/user-attachments/assets/fa5cfcbb-0336-4723-9728-9c3c4eb30c7c)
![df -h](https://github.com/user-attachments/assets/a7bcd60e-1638-4dd6-8632-ef7b2447510d)
![df -h](https://github.com/user-attachments/assets/682343a2-f66e-47ee-98fe-4e810623235f)
![df -h](https://github.com/user-attachments/assets/9e1db7aa-8cb3-4146-b471-6f41a56f215c)
![df -h](https://github.com/user-attachments/assets/f49e0175-fb79-4327-9af5-efaadf579f33)
![df -h](https://github.com/user-attachments/assets/60505f26-190a-48b5-8911-a8b3080e24f9)
![df -h](https://github.com/user-attachments/assets/bff8b0ca-8841-4034-8885-e8293f7559e7)
![df -h](https://github.com/user-attachments/assets/e523615e-ca1d-4f7c-883f-2372852596d4)


## Week 3
### Application Selection for Performance Testing 
3. Expected Resource Profiles documenting anticipated resource usage
4. Monitoring Strategy explaining measurement approach for each application

CPU-Intensive Workloads
stress-ng -Can generate configurable CPU stress by running multiple computation-heavy threads.
sysbench --test=cpu – Runs prime number calculations to measure raw CPU performance.

Memory-Intensive Workloads
stress-ng --vm – Allocates and manipulates large memory blocks to test RAM performance.
sysbench --test=memory – Measures sequential memory read/write throughput.

Disk and I/O Workloads
fio – Configurable tool for simulating read/write patterns.
dd if=/dev/zero of=testfile bs=1G count=1 oflag=dsync – Quick sequential write test.

Network Workloads
netperf – Tests various network performance metrics like latency and bandwidth.
ping / mtr – For latency and route stability checks.

![df -h](https://github.com/user-attachments/assets/4b28783f-b91b-4a29-94f8-da2dfa2cc434")
![df -h](https://github.com/user-attachments/assets/1962576a-7dc4-4aec-b068-1f2295449515)
![df -h](https://github.com/user-attachments/assets/79704fd8-0c3e-4bfe-9a5c-8120cbf6ae83)
![df -h](https://github.com/user-attachments/assets/10d0853c-ba14-4b9d-9492-b5bba7909b02)
![df -h](https://github.com/user-attachments/assets/1b752c9c-e01c-4f8b-b7f7-c0bc397175ce)
![df -h](https://github.com/user-attachments/assets/ec9d304e-448c-4cf5-8f08-ff84bcbe53c0)
![df -h](https://github.com/user-attachments/assets/9ae3f0dc-89ed-4ede-8462-378d3e98d3c3)
![df -h](https://github.com/user-attachments/assets/e8657cdd-3d44-400d-8414-697ad2fd45e7)
![df -h](https://github.com/user-attachments/assets/cf2d3ac5-c176-4cb1-b4e5-308510c5ecf5)



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

For your journal: Take screenshots showing process listings with visible command 
prompts. Explain what the different process states (R, S, D, Z, T) represent.

For your journal: Document the process lifecycle with examples. Explain when you would 
use foreground vs background processes, and the difference between kill and kill -9.


(To get ssh to work on ubuntu I had to install it first using:
sudo apt-get install openssh-server
as it is not automatically installed)


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
https://unix.stackexchange.com/questions/781711/cant-start-sshd-on-ubuntu-server-sshd-service-does-not-exist-despite-clearly
<img width="596" height="277" alt="Screenshot 2026-01-08 194429" src="https://github.com/user-attachments/assets/be8784f8-bd26-4b07-8bdf-b27a9510f659" />
<img width="434" height="263" alt="Screenshot 2026-01-08 194414" src="https://github.com/user-attachments/assets/b96ad45a-45ee-4613-8f56-1d6a9894a6af" />
<img width="586" height="301" alt="Screenshot 2026-01-08 194340" src="https://github.com/user-attachments/assets/ba713127-3d3c-44f7-82d5-f3e257f66144" />
<img width="556" height="316" alt="Screenshot 2026-01-08 193300" src="https://github.com/user-attachments/assets/77acfe99-3da6-4653-86af-0eafb09e759a" />
<img width="504" height="316" alt="Screenshot 2026-01-08 193123" src="https://github.com/user-attachments/assets/89d648bf-8024-45d0-96e4-1aa5c1e75494" />
<img width="454" height="73" alt="Screenshot 2026-01-08 192616" src="https://github.com/user-attachments/assets/b3a5d27e-1a3b-4844-a952-eb4e0b19408c" />

<img width="502" height="82" alt="Screenshot 2026-01-08 192021" src="https://github.com/user-attachments/assets/836649d8-71b4-4674-b91a-4a9afc6b835c" />
<img width="596" height="343" alt="Screenshot 2026-01-08 192006" src="https://github.com/user-attachments/assets/a5502a1c-e998-4827-bab5-b14dff422ddf" />
<img width="538" height="314" alt="Screenshot 2026-01-08 191702" src="https://github.com/user-attachments/assets/165fe928-2cee-46ab-bbfa-ce421a38863d" />
<img width="547" height="230" alt="Screenshot 2026-01-08 191519" src="https://github.com/user-attachments/assets/8a7bd48f-0ba0-4e66-a15e-4d56659f4d89" />
<img width="451" height="179" alt="Screenshot 2026-01-08 185812" src="https://github.com/user-attachments/assets/b70c7d5d-a476-48d9-a10d-27246b0cceb4" />
<img width="595" height="245" alt="Screenshot 2026-01-08 185513" src="https://github.com/user-attachments/assets/a6c6732c-bc53-4dc3-9437-a8f45749def1" />
<img width="595" height="329" alt="Screenshot 2026-01-08 181230" src="https://github.com/user-attachments/assets/8eba4f5e-3e8b-4cc1-b642-e6e9641755fc" />




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

For your journal: Document AppArmor status with screenshots. Explain the structure of 
an AppArmor profile and the purpose of enforce vs complain modes
(file content wouldnt display when inputing directory path so i had to manually move to the directory first to view the file contents, tcpdump is in enforce mode which means policy violations are blocked and logged)

https://linuxcapable.com/how-to-enable-or-disable-apparmor-on-ubuntu-linux/
<img width="492" height="314" alt="Screenshot 2026-01-11 135707" src="https://github.com/user-attachments/assets/cd03f638-ed48-4924-a21c-17bc61352b50" />
<img width="484" height="314" alt="Screenshot 2026-01-11 135645" src="https://github.com/user-attachments/assets/eb7f1f00-6ecc-465c-8523-d17163a61f3b" />
<img width="488" height="315" alt="Screenshot 2026-01-11 135618" src="https://github.com/user-attachments/assets/4ee1d6f6-57a7-421e-8c34-05cd5a5f0d1a" />
<img width="487" height="338" alt="Screenshot 2026-01-11 135527" src="https://github.com/user-attachments/assets/73bba842-865c-42b4-8b1d-83fe3757cbc5" />
<img width="491" height="314" alt="Screenshot 2026-01-11 135128" src="https://github.com/user-attachments/assets/0a09bfb1-d79b-476c-864b-6a1654ca56b8" />
<img width="491" height="323" alt="Screenshot 2026-01-11 135111" src="https://github.com/user-attachments/assets/b11eb8d7-b66c-4891-9460-dd13533e6a53" />
<img width="489" height="320" alt="Screenshot 2026-01-11 135046" src="https://github.com/user-attachments/assets/5a2324a9-0b02-4f02-be3e-d5a19b0d899a" />
<img width="488" height="316" alt="Screenshot 2026-01-11 135031" src="https://github.com/user-attachments/assets/e1daf0b3-1b41-4107-b835-8bb657c49cef" />
<img width="494" height="302" alt="Screenshot 2026-01-11 134950" src="https://github.com/user-attachments/assets/d4e89c2b-05d2-4d27-a25d-de54523137eb" />
<img width="610" height="365" alt="Screenshot 2026-01-10 152229" src="https://github.com/user-attachments/assets/f4f5ec39-e689-43fb-b582-0f24f7b030b0" />
<img width="606" height="361" alt="Screenshot 2026-01-10 152215" src="https://github.com/user-attachments/assets/1cbc3fdc-042b-4cb4-940e-932ebef32ef9" />
<img width="604" height="361" alt="Screenshot 2026-01-10 152204" src="https://github.com/user-attachments/assets/ad7d1c60-ab07-4e88-81e3-fa37549ce795" />
<img width="602" height="359" alt="Screenshot 2026-01-10 152152" src="https://github.com/user-attachments/assets/b5773fe1-d6a0-4c9f-ba17-358ca087192d" />
<img width="608" height="361" alt="Screenshot 2026-01-10 152140" src="https://github.com/user-attachments/assets/185eb817-029a-41c0-b441-70556fffc50e" />
<img width="602" height="358" alt="Screenshot 2026-01-10 152127" src="https://github.com/user-attachments/assets/55065ff1-9e2a-4fd0-aeff-e93bb8a169b1" />
<img width="608" height="362" alt="Screenshot 2026-01-10 152103" src="https://github.com/user-attachments/assets/064aedff-1997-420b-9173-55cd40a436a6" />
<img width="610" height="245" alt="Screenshot 2026-01-10 151952" src="https://github.com/user-attachments/assets/8d1edcbf-e4af-4059-a4bc-740269773470" />
<img width="606" height="345" alt="Screenshot 2026-01-10 151938" src="https://github.com/user-attachments/assets/8ee89dc3-75d5-4d5a-822c-7a1628389f26" />
<img width="610" height="364" alt="Screenshot 2026-01-10 151922" src="https://github.com/user-attachments/assets/c7163486-d674-4354-a83d-e477c50b4de0" />
<img width="600" height="343" alt="Screenshot 2026-01-10 151910" src="https://github.com/user-attachments/assets/00d3b3b9-3943-434d-9dd9-849922239ddb" />
<img width="494" height="307" alt="Screenshot 2026-01-10 142508" src="https://github.com/user-attachments/assets/4f2b4ad1-1d6d-4204-a79e-5218e5df5a68" />
<img width="497" height="289" alt="Screenshot 2026-01-10 142332" src="https://github.com/user-attachments/assets/e4fce224-58f0-4e98-ae22-769f3a5ffa5e" />
<img width="488" height="311" alt="Screenshot 2026-01-10 142214" src="https://github.com/user-attachments/assets/2f533073-5c2c-4129-8cf6-9b4b88759b00" />
<img width="572" height="305" alt="Screenshot 2026-01-10 135409" src="https://github.com/user-attachments/assets/8d6a94fc-c7f6-43ef-a997-a0f80c05afdd" />
<img width="569" height="313" alt="Screenshot 2026-01-10 135300" src="https://github.com/user-attachments/assets/9991bea7-f8d8-4c2a-9d01-926996cda23a" />
<img width="571" height="227" alt="Screenshot 2026-01-10 135215" src="https://github.com/user-attachments/assets/2f623b5e-1a5c-40bc-9560-3c2ffc61417b" />
<img width="578" height="322" alt="Screenshot 2026-01-10 135159" src="https://github.com/user-attachments/assets/d9871551-7c12-4de3-95a9-fa3d998387ea" />
<img width="491" height="316" alt="Screenshot 2026-01-11 145608" src="https://github.com/user-attachments/assets/f4ecd1e6-ad3a-4668-a33a-6ca379644c32" />


<img width="491" height="287" alt="Screenshot 2026-01-09 175438" src="https://github.com/user-attachments/assets/3601c5bd-2b89-4196-ac6a-7a656c5ec0c9" />
<img width="488" height="107" alt="Screenshot 2026-01-09 171251" src="https://github.com/user-attachments/assets/973129e5-2a14-4635-b0cf-6d6d72912667" />
<img width="142" height="48" alt="Screenshot 2026-01-09 170800" src="https://github.com/user-attachments/assets/e596bd46-5b2b-4bea-98a6-35e15ced1c05" />
<img width="447" height="303" alt="Screenshot 2026-01-09 165007" src="https://github.com/user-attachments/assets/01fed95f-5f36-4548-ae86-865ba6d5aa32" />
<img width="492" height="254" alt="Screenshot 2026-01-09 164953" src="https://github.com/user-attachments/assets/08001d38-57f3-4c47-8a97-7d48eb08e117" />
<img width="575" height="330" alt="Screenshot 2026-01-09 164909" src="https://github.com/user-attachments/assets/bee9bd7c-1f0d-4532-8671-ce0d80040658" />
<img width="488" height="313" alt="Screenshot 2026-01-11 135726" src="https://github.com/user-attachments/assets/1fe35c1c-6480-4edc-b030-3d3b90078b5c" />


week8 lab activity pdf
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
<img width="404" height="259" alt="Screenshot 2026-01-11 155124" src="https://github.com/user-attachments/assets/3a6568d4-e0d0-4632-974f-01c243a304d2" />
<img width="406" height="262" alt="Screenshot 2026-01-11 155026" src="https://github.com/user-attachments/assets/5f4719c6-76b1-499e-bfba-86619b61de07" />
<img width="493" height="41" alt="Screenshot 2026-01-11 154006" src="https://github.com/user-attachments/assets/88c8f7e9-e535-48b4-9cd3-ca8fe78af7dd" />
<img width="269" height="112" alt="Screenshot 2026-01-11 153430" src="https://github.com/user-attachments/assets/04fe4e1d-03bb-4052-be30-9e71edd953b8" />
<img width="488" height="241" alt="Screenshot 2026-01-11 153008" src="https://github.com/user-attachments/assets/6d209c23-ab82-4eef-b6f9-4f1b511bd2e6" />
<img width="488" height="315" alt="Screenshot 2026-01-11 152447" src="https://github.com/user-attachments/assets/6ec3e80b-ce26-4c73-9516-e04f4b7d977c" />

