# rosserial_mac


an docker contanter run at mac .
docker for mac do not map /dev to container /dev

##
modify SerialClient.py 
self.port = serial_for_url(port, baud, timeout=self.timeout*0.5)



rosrun rosserial_python serial_node.py socket://192.168.65.2:7777

192.168.65.2  is docker.for.mac.localhost


mac run 
python3 tcp_serial_redirect.py  /dev/cu.wchusbserial14540 57600



tcp_serial_redirect.py from pyserial

