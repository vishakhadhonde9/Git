# Secure Shell on CLI -
- SSH (Secure Shell) is a way to securely connect to another computer or server over a network, like logging into a remote machine.

# Key-pair generation -

          ssh-keygen -t rsa -b 2048


- Two files are created:
   - Private key: id_rsa (keep this safe and never share it).
   - Public key: id_rsa.pub (this is shared with the server).
