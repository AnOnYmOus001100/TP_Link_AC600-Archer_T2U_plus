# Driver for Debian Based Linux Distros (Ubuntu/Kali Linux)(x86_64)

## 1. Update apt :
$ sudo apt update

## 2. Install dkms and git :
$ sudo apt install dkms git

## 3. Install Build Dependencies:
$ sudo apt install build-essential libelf-dev linux-headers-$(uname -r)

## 4. Download the Driver files using git :
$ git clone https://github.com/aircrack-ng/rtl8812au.git

## 4. Navigate to the cloned directory rtl8188au :
$ cd rtl8812au

## 5. Build and Install the Driver :
$ sudo make dkms_install

* if the installation gets aborted , type: 
$ sudo dkms remove 8812au/5.6.4.2_35491.20191025 --all'''
* if errors pop up:
'''Usage: remove / --all'''

## 6. Plug the adapter into the USB.

## 7. Check the wireless interfaces:
$ iwconfig

** Note: This driver is by aircrackng and its supports monitor mode.
