# Lab 2
## Using a camera on Raspberry Pi
Using a USB camera on the Pi, and restarting the Pi, we can use this command line to take a single image frame from the webcam:

ffmpeg -f v4l2 -video_size 1280x720 -i /dev/video0 -frames 1 out.jpg

![6](https://user-images.githubusercontent.com/68234338/158932115-c4ab79fd-06dc-4b08-ad84-4f47a7e80803.jpg)
![7](https://user-images.githubusercontent.com/68234338/158932117-00e8978f-77d4-4b77-815e-0fbecc002963.jpg)
![8](https://user-images.githubusercontent.com/68234338/158932118-a956f291-5868-4f16-8a08-e38c17b29311.jpg)
