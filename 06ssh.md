Generate Host Keys: You can generate SSH host keys using the ssh-keygen command:
# sudo ssh-keygen -A
      or
# ssh-keygen 
for generating ssh public key in your specified directory;
# ssh-copy-id user1@ip                               
# sudo service ssh start  

# sudo service ssh status

Enable SSH Service (Optional):
If you want the SSH service to start automatically at boot time, you can enable it using:
# sudo service ssh enable

Verify SSH Connectivity:
After starting the SSH service, try connecting to your system via SSH from another machine to ensure that the SSH service is functioning correctly:
# ssh username@hostname_or_ip

    Replace username with your actual username and hostname_or_ip with the hostname or IP address of your Ubuntu system.

    Check SSH Configuration: Ensure that the SSH server (sshd) configuration allows password authentication. Edit the SSH configuration file /etc/ssh/sshd_config:

# sudo nano /etc/ssh/sshd_config
Look for the line PasswordAuthentication and make sure it's set to yes. If the line is commented out with a #, remove the # to enable it. Save the changes and exit the editor.
Restart SSH Service: After modifying the SSH configuration, restart the SSH service to apply the changes:

# sudo service ssh restart







