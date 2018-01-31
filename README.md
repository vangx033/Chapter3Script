#!/bin/bash
#Xee Ho Vang 
#Chapter 3 script

echo "Here is my script for chapter 3."

#list what are in the /dev
ls /dev

#change directory to /dev and check where am I
cd /dev
pwd

#Testing the kernel if it ignores the input and view devices
echo Hi there > /dev/null
ls -l

#showing the path for the device sda
udevadm info --query=all --name=/dev/sda

#monitoring all the devices
udevadm monitor

#change directory back to home and display a closing statement
cd
echo "Good bye and have a nice day"
