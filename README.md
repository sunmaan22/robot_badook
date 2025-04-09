# robot_badook

ssh sunmaan@172.20.10.6
qwer1234

--------------------------------------------------------

ssh -X sunmaan@172.20.10.6
export DISPLAY=172.20.10.2:0.0

--------------------------------------------------------

sudo chmod 666 /dev/ttyS0
minicom -D /dev/ttyS0 -b 9600

--------------------------------------------------------

sudo systemctl stop serial-getty@ttyS0.service
sudo systemctl disable serial-getty@ttyS0.service

--------------------------------------------------------

roscore
chmod +x ~/catkin_ws/src/gps_pkg/scripts/gps_publisher.py
rosrun gps_pkg gps_publisher.py
