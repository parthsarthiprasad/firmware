ath10k-firmware
===============

These are the latest firmware files for ath10k, a mac80211 driver for
QCA988x, QCA6174, QCA99XX and similar. The official location to
download ath10k images is from linux-firmware:

https://git.kernel.org/cgit/linux/kernel/git/firmware/linux-firmware.git/

For more information check the wiki:

http://wireless.kernel.org/en/users/Drivers/ath10k/firmware

--- 
---

> this repository is used to save a backup of firmware
### steps to install firmware
1.`$ sudo apt-get update`
2.`$ sudo apt-get install git`
3.`$ git clone https://github.com/kvalo/ath10k-firmware.git`
4.`$ sudo mkdir /lib/firmware/ath10k/QCA9377`
5.`$ sudo mkdir /lib/firmware/ath10k/QCA9377/hw1.0`
6.`$ cd ath10k-firmware/QCA9377/hw1.0`
7.`$ sudo cp *  /lib/firmware/ath10k/QCA9377/hw1.0`
8.`$ cd /lib/firmware/ath10k/QCA9377/hw1.0`
9.`$ sudo mv WLAN.TF.1.0/firmware-5.bin_WLAN.TF.1.0-00267-1     ./firmware-5.bin`

#### other drivers do not work as after kernel update 4.2 , dur to implicit function definition error (can be fixed by adding including few other header files), (mentioned in docs) .
