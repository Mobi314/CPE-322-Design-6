# Lab 8
## Data Analysis

## 1: Installing Packages

$ sudo apt update

$ sudo apt install python3-scipy

$ sudo apt install python3-matplotlib

$ sudo apt install python3-pandas

$ sudo apt install libopenblas-dev

$ sudo apt install libatlas-base-dev

$ sudo pip3 install -U numpy

$ sudo pip3 install --only-binary :all: -U scikit-learn

$ sudo pip3 install -U tensorflow

$ sudo pip3 install -U keras==2.3.1

## 2: Installing Packages:

$ cd ~/demo

$ cp ~/iot/lesson8/plt_final.py .

$ cp ~/iot/lesson8/plt_cv2.py .

$ nano plt_final.py

data = read_csv('rpidata.csv')

$ nano plt_cv2.py

X = read_csv('rpidata.csv', usecols=[1])

y = read_csv('rpidata.csv', usecols=[2])

$ python3 plt_final.py

$ python3 plt_cv2.py

![1](https://user-images.githubusercontent.com/68234338/166811373-c0094a0b-b31e-43d6-ac2a-e11a282c22f5.jpg)

![2](https://user-images.githubusercontent.com/68234338/166811375-a7ecd89d-1878-4049-956d-fc280379fa19.jpg)
