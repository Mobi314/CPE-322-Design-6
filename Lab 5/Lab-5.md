# Lab 5
## Installing and using Crossbar.io and Paho

## 1: Installing Eclipse Mosquitto:

$ sudo apt update

$ sudo apt install mosquitto mosquitto-clients

$ mosquitto_sub -h localhost -v -t "\$SYS/#"

$ service mosquitto status

$ netstat -tln

$ mosquitto_sub -h localhost -v -t test/topic &\

$ mosquitto_pub -h localhost -t test/topic -m "Hello"
 
![1](https://user-images.githubusercontent.com/68234338/164990059-bfc656ef-3097-4333-bd31-19eebfc76c85.jpg)
 
![2](https://user-images.githubusercontent.com/68234338/164990081-d95df8d6-d6f1-40af-9be8-4e06a57e6b43.jpg)

## 2: Intall Paho and run code to subscribe on one terminal and publish on another

$ sudo pip3 install -U paho-mqtt

$ git clone https://github.com/eclipse/paho.mqtt.python.git

$ cd ~/iot/lesson5

$ python3 client.py

Terminal 1 (press control-c to stop)

$ python3 sub.py

Terminal 2

$ python3 pub.py

Terminal 1 (press control-c to stop)

$ python3 sub-multiple.py

Terminal 2

$ python3 pub-multiple.py

Terminal 1 (press control-c to stop)

$ python3 subcpu.py

Terminal 2

$ python3 pubcpu.py

![3](https://user-images.githubusercontent.com/68234338/164990839-625ba845-8c61-41de-8a8d-a2fdf4d80725.jpg)

![4](https://user-images.githubusercontent.com/68234338/164990841-d7fa5aba-26e4-4de6-a71d-17943f143123.jpg)

