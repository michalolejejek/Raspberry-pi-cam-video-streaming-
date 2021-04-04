# Raspberry-pi-cam-video-streaming-

You can use it to stream video by your RPi via HTTP server.

## Needed Hardware

* Raspberry Pi (any model with camera socket)
* Dedicated camera
* Local network (Wifi or Lan)
* Another device with the possibility of web browsing

## Needed Software

* python3 on raspi
* pip
* picamera (library)

## Setup
First of all you should enable camera port on your rpi.
```
$ sudo raspi-config

>Interfacing Options
>Camera
>enable
```
After this operation you should reboot your device.

Next, you should install picamera library for python3

`$ sudo apt-get install python-picamera python3-picamera`

Clone repo

`$ git clone https://github.com/michalolejejek/Raspberry-pi-cam-video-streaming-.git`

`$ cd Raspberry-pi-cam-video-streaming-`

## Running 

On your raspberry:

`~/Raspberry-pi-cam-video-streaming- $ python3 video_streaming.py`

On your computer or mobile phone type in browser:

`http://<your_raspperry_ip>:8000`

for example:

`http://192.168.43.127:8000`


### How to see ip of your raspberry
On your raspberry type this:
`$ hostname -I`

