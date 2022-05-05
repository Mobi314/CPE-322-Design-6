# Lab 9: Yang

## Install & Run pyang and PlantUML:

On Raspbery Pi

Install and run pyang:

$ sudo apt install libxml2-dev libxslt1-dev

$ sudo pip3 install -U lxml pyang

$ cp ~/iot/lesson9/intrusiondetection.yang ~/demo

$ cd ~/demo

$ cat intrusiondetection.yang

$ pyang -f yin -o intrusiondetection.yin intrusiondetection.yang

$ cat intrusiondetection.yin

$ pyang -f uml -o intrusiondetection.uml intrusiondetection.yang --uml-no=stereotypes,annotation,typedef

$ cat intrusiondetection.uml

Install PlantUML:

$ sudo pip3 install -U plantuml

Run PlantUML to create a sequence diagram in PNG:

$ python3 -m plantuml intrusiondetection.uml

Install and run GIMP and Pinta to display a PNG file via VNC Viewer:

$ cd

$ sudo apt update

$ sudo apt install gimp pinta

$ cd ~/demo

$ pinta intrusiondetection.png

$ gimp -h

$ gimp -a intrusiondetection.png

![1](https://user-images.githubusercontent.com/68234338/166989964-75974694-a2d0-4ef4-af9a-cb0d457c47b7.jpg)

![2](https://user-images.githubusercontent.com/68234338/166989969-fffbec94-75ee-4d06-96c4-6111721ccc3a.jpg)

![3](https://user-images.githubusercontent.com/68234338/166989972-272c9c50-238f-4408-a13a-6eb311fd99e5.jpg)

![D1](https://user-images.githubusercontent.com/68234338/166990074-0ff0ca07-c367-4d74-8a8b-3c6080021f07.jpg)

![D2](https://user-images.githubusercontent.com/68234338/166990080-465b6fbd-1a2d-495a-b656-4a4f1dc0122f.jpg)
