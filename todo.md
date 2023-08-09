add sudo user to sudoers file
usermod -aG sudo username
* Enable BT Audio on X1 Carbon
touch /etc/modprobe.d/iwlwifi.conf
* Add line to file
options iwlwifi bt_coex_active=0
* reboot
* After reboot check contents of /sys/module/iwlwifi/parameters/bt_coex_active

cat /sys/module/iwlwifi/parameters/bt_coex_active
* you should see the following:
  
N

*Install snap store
