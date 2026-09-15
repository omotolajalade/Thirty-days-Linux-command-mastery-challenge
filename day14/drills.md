Day 14 drill:On an Amazon Linux or RHEL box, install a package with dnf, confirm it with rpm -qa, then
compare the workflow against the equivalent apt steps from Day 13


Step 1 — Install package with dnf

sudo dnf install -y tree


Step 2 — Confirm with rpm

rpm -qa | grep tree

Step 3 — Test the package

tree /etc --dirsfirst | head -20

Step 4 — Compare workflow to Day 13's apt

Step	apt (Day 13)	         dnf (Day 14)
Install	sudo apt install             tree	sudo dnf install -y tree
Confirm install	dpkg -l | grep tree	        rpm -qa | grep tree
	To test dpkg -l | grep cowsay             tree /etc --dirsfirst | head -20
