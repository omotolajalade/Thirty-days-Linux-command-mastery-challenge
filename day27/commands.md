Commands and what they do

1. ssh: connect to a remote machine.

2. ssh -p: connect using a non-default port (SSH normally uses port 22).

3. ssh -i: connect using a specific private key file (also used earlier with your .pem file).

4. ssh-keygen: generate a new SSH key pair (public + private key).

This creates two files: a private key (keep secret, never share) and a public key ending in .pub (safe to share/copy to servers)

5. ssh-copy-id: copy your public key to a remote server, enabling password-free login.

6. scp: securely copy a file to/from a remote host.

The secure copy command uses the same encrypted connection as SSH.

7. sftp: an interactive file-transfer session (like FTP, but secure).

8. rsync: a smarter, more efficient copy tool — only transfers what's changed.

9. ~/.ssh/config: a config file letting you save connection shortcuts.

10. sshd_config hardening: the server-side SSH configuration file (/etc/ssh/sshd_config), where you'd disable password login, change the default port, etc. 
Note: Editing this on a remote server incorrectly can lock you out — always keep a second connection open when testing changes.