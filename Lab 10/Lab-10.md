# Lab 10: Blockchain

## Hash function with randomization

### Run hash_value.py twice and compare results

$ cd ~/iot/lesson10

$ cat hash_value.py

$ python3 hash_value.py

$ python3 hash_value.py

![1](https://user-images.githubusercontent.com/68234338/166998411-acb04d9e-139b-408b-8e63-ca3bfa950948.jpg)

### Build the tiniest blockchain in less than 50 lines of Python by Gerald Nash (2017-07-16)

$ cd ~/iot/lesson10

$ cat snakecoin.py

$ python3 snakecoin.py

![2](https://user-images.githubusercontent.com/68234338/167001008-3e87faac-b2fe-4312-8c3d-160d4a2cef04.jpg)

![3](https://user-images.githubusercontent.com/68234338/167001013-062e0676-cb5e-4d7e-a819-8ec7c7b9800d.jpg)


### Let’s Make the Tiniest Blockchain Bigger Part 2: With More Lines of Python by Gerald Nash (2017-07-23)

**Terminal 1: Run the SnakeCoin server at http://127.0.0.1:5000/ (Press Ctrl+C to quit)**

$ cat snakecoin-server-full-code.py

$ python3 snakecoin-server-full-code.py

$ cd

**In case of ImportError: cannot import name 'soft_unicode' from 'markupsafe'**

$ sudo pip3 install markupsafe==2.0.1

$ python3 snakecoin-server-full-code.py

![4](https://user-images.githubusercontent.com/68234338/167030022-cd840024-9bad-4c04-a869-c3fa4951a4cf.jpg)

![5](https://user-images.githubusercontent.com/68234338/167030025-03ef939e-962b-48d6-ac01-4fb3ab1d1900.jpg)

**Installing PyOTA**

$ sudo pip3 install pyota[ccurl]

$ cd ~/iot/lesson10

$ cat iri_node_info.py

$ python3 iri_node_info.py

$ cd

![6](https://user-images.githubusercontent.com/68234338/167034563-72d1d2d5-5baa-470b-b287-4166d88a2f35.jpg)
