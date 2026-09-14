Day 9: Generate a SHA-256 checksum for a downloaded file to verify its integrity, make a file immutable
with chattr, then open only port 22 and port 443 on the firewall.

Step 1: Create a simple file that you will use throughout the exercise. This gives you something safe to hash, encrypt, and protect.

Step 2: Use md5sum on the file. This creates a fingerprint of the file that you can use to check whether its contents change.

Step 3: Use sha256sum on the same file. Compare it with the MD5 result and notice that they produce different types of fingerprints.

Step 4: Use gpg --gen-key to create your GPG key. Follow the prompts provided by Linux. This key will be used for encryption and decryption.

Step 5: Use gpg --encrypt to encrypt your test file. The result should be an encrypted GPG file that cannot be read normally.

Step 6: Use gpg --decrypt to decrypt the encrypted file and return it to a readable form.

Step 7: Use chattr +i on your test file. This makes the file protected from normal modification or deletion.

Step 8: Use lsattr to confirm that the immutable attribute has been added to the file.

Step 9: Use sudo ufw enable to turn on the UFW firewall. UFW means Uncomplicated Firewall.

Step 10: Allow port 22 for SSH and port 443 for HTTPS using UFW. These are the two ports required by your Day 9 drill.

Step 11: Use sudo ufw status to confirm that UFW is active and that your allowed ports appear in the firewall rules.
