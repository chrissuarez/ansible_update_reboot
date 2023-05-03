# ansible_update_reboot
Update and reboot Ubuntu hosts when needed

Commands

ssh-keygen -t ed25519 -C "your_email@example.com"
cat ~/.ssh/id_ed25519.pub >> ~/.ssh/authorized_keys
chmod 600 ~/.ssh/authorized_keys

Test access with: ssh chris@localhost

sudo crontab -e

30 3 * * * /usr/bin/ansible-pull -U https://github.com/chrissuarez/ansible_update_reboot.git update_and_reboot.yml
