# ansible_update_reboot
Update and reboot Ubuntu hosts when needed

Commands

ssh-keygen -t ed25519 -C "your_email@example.com" <br>
cat ~/.ssh/id_ed25519.pub >> ~/.ssh/authorized_keys <br>
chmod 600 ~/.ssh/authorized_keys <br>
 <br>
 <br>
Test access with: ssh chris@localhost <br>
 <br>
sudo crontab -e <br>
 <br>
30 3 * * * /usr/bin/ansible-pull -U https://github.com/chrissuarez/ansible_update_reboot.git update_and_reboot.yml<br>
<br>
Create the file called "chris" in "/etc/sudoers.d" with the following line:<br>
chris ALL=(ALL) NOPASSWD: ALL
