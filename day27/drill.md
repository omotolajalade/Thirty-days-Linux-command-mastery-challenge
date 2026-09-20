Day 27 drill: Generate an SSH key pair, copy the public key to a remote host, connect without a password, then
securely copy a file to and from that server.

Step 1 — Generate a key pair

ssh-keygen -t ed25519

Step 2 — Copy your public key to a remote host
ssh-copy-id -i ~/.ssh/id_ed25519.pub ec2-user@your-ec2-ip

Step 3 — Connect without a password

ssh ec2-user@your-ec2-ip

Step 4 — Securely copy a file to the server, then back

echo "test file" > testfile.txt
scp testfile.txt ec2-user@your-ec2-ip:/home/ec2-user/
scp ec2-user@your-ec2-ip:/home/ec2-user/testfile.txt ./retrieved.txt