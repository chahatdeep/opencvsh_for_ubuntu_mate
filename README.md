# opencvsh_for_ubuntu_mate


Step 1. Download ubuntu mate image from

http://odroid.in/ubuntu_16.04lts/

Step 2. un xz on your host with this command

unxz ubuntu-16.04-mate-odroid-xu3-20160708.img.xz

Step 3. Insert micro-SD Card to your host PC

Step 4. Copy img to SDCARD

replace sdX to your SDCARD device name in your host - Be carefull!!

sudo dd if=ubuntu-16.04-mate-odroid-xu3-20160708.img of=/dev/sdX bs=1M conv=fsync
	sync

Step 5. Turn off the Odroid and Put your SDCARD into Odroid

Step 6. Move the switch to uSD from emmc and Turn on the board

Step 7. login your target(User:odroid, PW: odroid)

Step 8. on your target : run any web-browser and connect to

https://github.com/nanuyo/opencvsh_for_ubuntu_mate

Step 9: and download opencv_install_to_ubuntu_mate_16.04.sh


Step 10. run script
source opencv_install_to_ubuntu_mate_16.04.sh

Step 11. Test facedetect sample

cd opcv-2.13.xx/samples/c
./facedetect lena.jpg

