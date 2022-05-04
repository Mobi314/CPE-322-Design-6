# Lab 7
## Installing and using ThingSpeak and Google Cloud Platform

## 1: Signing up for & Using ThingSpeak:

Sign up and log in ThingSpeak

Create new channel cpu_loop with field1 cpu_pc and field2 mem_avail_mb

Copy the Write API Key from channels

Review and run thingspeak_feed.py

$ sudo pip3 install -U psutil

$ cd ~/demo

$ cp ~/iot/lesson7/thingspeak_cpu_loop.py .

$ cp ~/iot/lesson7/thingspeak_feed.py .

$ cat thingspeak_cpu_loop.py

$ cat thingspeak_feed.py

$ python3 thingspeak_feed.py

An API key savefile was not found. Enter Write API Key >>>

Should we save this key for future use? [y/N] >>>

![1](https://user-images.githubusercontent.com/68234338/166794456-a7448fbd-c931-4d6a-bb39-8319ad3e7f04.jpg)

![3](https://user-images.githubusercontent.com/68234338/166794917-82a2830d-650f-48a9-88aa-c1093b714065.jpg)

![4](https://user-images.githubusercontent.com/68234338/166795093-c2213eb0-764c-407e-a5c7-b6173b6ea0e1.jpg)

![2](https://user-images.githubusercontent.com/68234338/166795262-1da6525c-2ba3-4982-be74-8ff38f0cec00.jpg)

## 2: Logging into Google Cloud Platform Identity and Access Management & Using Google Sheets:

Sign up and log in the Google Cloud Platform Identity and Access Management (IAM)

Click "Create" and enter the project name, e.g., rpidata

≡ > APIs & Services > + Enable APIs & Services > Enable both Drive API and Sheets API

Credential > Create Credentials > Create service account key > Service account > rpidata > JSON key type > Create > download  rpidata-xxxxxxxxxxxx.json

Install gspread and oauth2client

$ sudo pip3 install -U gspread oauth2client

Copy system_info.py and rpi_spreadsheet.py to ~/demo

On Raspberry Pi OS (Bullseye), change /opt/vc/bin/vcgencmd to /usr/bin/vcgencmd in system_info.py

$ cd demo

$ cp ~/iot/lesson3/system_info.py .

$ cp ~/iot/lesson7/rpi_spreadsheet.py .

If the JSON key file (* = xxxxxxxxxxxx) is on a different computer, secure copy it to the same directory as rpi_spreadsheet.py

$ scp rpidata-*.json pi@192.168.x.xxx:/home/pi/demo

If the the JSON key file is on a Raspberry Pi, move it to the same directory as rpi_spreadsheet.py

$ mv ~/Downloads/rpidata-*.json ~/demo

Go to Google Sheets

Start a new spreadsheet rpidata

Share the spreadsheet with the "client_email" address in the .json file, select “Can edit,” and click "Send"

May receive an email with the subject "Delivery Status Notification (Failure)" and the message "Address not found" from  mailer-daemon@google.com

Delete Rows 2 to 1000, and enter Date / Time, CPU Usage %, Temperature C to header cells

This deletion is not necessary with the improved rpi_worksheet.py and cpu_worksheet.py that can check the next empty row to write data

Edit rpi_spreadsheet.py

$ nano rpi_spreadsheet.py

GDOCS_OAUTH_JSON = 'rpidata-xxxxxxxxxxxx.json'

GDOCS_SPREADSHEET_NAME = 'rpidata'

Run rpi_spreadsheet.py

$ python3 rpi_spreadsheet.py

![5](https://user-images.githubusercontent.com/68234338/166801406-332877d7-ba7a-4a3b-a4d2-82ef97dd101d.jpg)

![6](https://user-images.githubusercontent.com/68234338/166801407-c354f418-b31d-4093-8bde-81c6a469bd37.jpg)

![7](https://user-images.githubusercontent.com/68234338/166801410-ef0f9f1b-a98b-4969-b674-e22589882d4f.jpg)
