| Command and What it does 

md5sum: Creates an MD5 checksum to help check if a file has changed.
NOTE: MD5 means Message-Digest Algorithm 5 which is to creates a fingerprint of a file so you can check whether it changed.

sha256sum: Creates a SHA-256 checksum for checking file integrity.
NOTE: SHA-256 means Secure Hash Algorithm 256-bit it is used to create a stronger file fingerprint than MD5.

gpg --gen-key: Creates a GPG key pair for encryption and digital security.
NOTE: GPG means GNU Privacy Guard which is a tool used for encryption, decryption, and digital signatures.

gpg --encrypt: Encrypts a file so it cannot be easily read without the required key.

gpg --decrypt: Decrypts an encrypted GPG file back into readable form.

chattr +i: Makes a file immutable, meaning it cannot normally be modified or deleted.
NOTE: chattr +i → chattr means change file attributes, while +i means add the immutable attribute.

lsattr Shows special attributes assigned to files.
NOTE: lsattr → ls means list, and attr means attributes, so it lists file attributes 

ufw enable: Turns on the UFW firewall.
NOTE: UFW means Uncomplicated Firewall which is a simple tool used to control network connections on Linux.

ufw allow: Allows specified network traffic through the firewall.     

ufw status: Shows whether the firewall is active and displays its rules.