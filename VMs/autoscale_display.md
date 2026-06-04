sudo apt install open-vm-tools    # Debian/Ubuntu
sudo yum install open-vm-tools   # RHEL/CentOS

or

xrandr --output $(xrandr | grep " connected" | awk '{print $1}') --mode 1920x1080
