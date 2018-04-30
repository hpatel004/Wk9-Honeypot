# Week 9 - Honeypot

Time spent: 10 hours spent in total

> Objective: Setup a honeypot and provide a working demonstration of its features.

### Required: Overview & Setup

- [x] I deployed MHN in an UBUNTU 14.04 instance using Google Cloud Services with the following honeypots: shockpot, Dionaea, snort, suricata, p0f, elastichoney.
- [x] The setup:
  - create a gcloud account and a project
  - in the cloud launcher, select Ubuntu Trusty (14, because the newer versions don't work)
  - allow HTTP traffic and all ports
  - in Compute Engine, select the VM instance and open SSH in a separate browser window
  - in the opened window, install MHN by executing the following commands:
      sudo apt-get update
      sudo apt-get install git -y
      $ cd /opt
      $ sudo git clone https://github.com/RedolentSun/mhn.git
      $ cd mhn
      $ sudo ./install.sh
  - whenever prompted, answer n or blank
### Required: Demonstration

- [x] I used nmap to scan the networknmap
- [x] An example of the data captured by the honeypot (example: IDS logs including IP, request paths, alerts triggered)
![1](https://user-images.githubusercontent.com/31852525/39412998-11033818-4bd9-11e8-92c5-b0eab2d2bb28.gif)

### Stretch Features
- Honeypot
	- [ ] HTTPS enabled (self-signed SSL cert)
	- [ ] A web application with both authenticated and unauthenticated footprint
	- [ ] Database back-end
	- [ ] Custom exploits (example: intentionally added SQLI vulnerabilities)
	- [ ] Custom traps (example: modified version of known vulnerability to prevent full exploitation)
	- [ ] Custom IDS alert (example: email sent when footprinting detected)
	- [ ] Custom incident response (example: IDS alert triggers added firewall rule to block an IP)
- Demonstration
  
	- [ ] Additional attack demos/writeups
	- [x] Captured malicious payload (see above)
	- [ ] Enhanced logging of exploit post-exploit activity (example: attacker-initiated commands captured and logged)
