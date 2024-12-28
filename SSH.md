# Secure Shell on CLI -
- SSH (Secure Shell) is a way to securely connect to another computer or server over a network, like logging into a remote machine.

# Key-pair generation -

          ssh-keygen -t rsa -b 2048


- Two files are created:
   - Private key: id_rsa (keep this safe and never share it).
   - Public key: id_rsa.pub (this is shared with the server).
- Verify : cd .ssh and ls -a

- **Set Permissions for the Key Pair File -**
- The .pem file (private key) should be kept secure. You must set the correct permissions for it before using it to connect


          chmod 400 /path/to/your-key.pem

- **SSH into the EC2 Instance -**
- To connect to your EC2 instance via SSH, use the following command


         ssh -i /path/to/your-key.pem ec2-user@<your-instance-public-ip>
