# <center> Practice Set for Linux System Administration - SSH </center>

1. ## Configure SSH
   
    - check ip addresses on both machines
      ```bash
      ip addr show
      ```
    - create new SSH key on Ubuntu workstation
      ```bash 
      cd .ssh 
      ssh-keygen -b 4096 -C "<descriptor>"
      chmod 600 id_rsa
      ```
    - Copy SSH Public key to Alma server
      ```bash
      ssh-copy-id -i ~/.ssh/id_rsa.pub <name>@<ip>
      ```
    - Test SSH connection from  ubuntu => Alma
      ```bash
      ssh <name>@<ip>
      ```

    - Deny SSH Password authentication 
    -  Troubleshooting SSH
       -  Ensure correct permissions are set on files and .ssh folders (700)
       -  Is public key authentication allowed in /etc/ssh/sshd_config?
  

    
 