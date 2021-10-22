# stanford-ilabs-rpi-project
Using Raspberry Pi cameras to create an iLab.

# Installation
Clone this repo onto the host and onto any pi cameras (make sure it is cloned in the /home/pi directory)

You may need to add some python packages if you don't have them already (Anaconda is the recommended command line interface for this program because it is easy to install missing packages) 

Find the [ip address](https://www.raspberrypistarterkits.com/how-to/find-raspberry-pi-ip-address/) of each Pi and put them in the [pi_ip.txt](https://github.com/Mattias421/stanford-ilabs-rpi-project/blob/main/pi_ip.txt).

Generate and authorize [ssh keypairs](https://www.raspberrypi.com/documentation/computers/remote-access.html) and write the location of each private key location in [ssh_loc.txt](https://github.com/Mattias421/stanford-ilabs-rpi-project/blob/main/ssh_loc.txt). (WARNING: keys must match their corresponding Pi in pi_ip.txt). It is advised to set up [passwordless ssh](https://raspi.tv/2012/how-to-set-up-keys-and-disable-password-login-for-ssh-on-your-raspberry-pi) so that you don't have to enter passwords for each photo taken.

# Getting started
An example command is: main.py --experiment_name "objects" --num_variables 1 

This will set up a 1 camera experiment with 1 variable called "objects". (make sure not to use and resticted characters or spaces)

# The end result
There will be a [CSV](https://github.com/Mattias421/stanford-ilabs-rpi-project/blob/main/experiments/objects/objects.csv) explaining which variables apply to which photo. The experiment photos can be found in the [photos folder](https://github.com/Mattias421/stanford-ilabs-rpi-project/tree/main/experiments/objects/photos) of each experiment. Photos are also saved to each Pi.

![legoman_photo](/experiments/objects/photos/photo1_cam2.jpg)
