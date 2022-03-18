# Lab 2
## Using a camera on Raspberry Pi
Using a USB camera on the Pi, and restarting the Pi, we can use this command line to take a single image frame from the webcam:
ffmpeg -f v4l2 -video_size 1280x720 -i /dev/video0 -frames 1 out.jpg

