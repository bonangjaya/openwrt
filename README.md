Building & Install OSCAM
========================
sudo apt-get update && sudo apt-get upgrade -y
sudo apt-get install cvs subversion libusb-1.0

svn checkout http://www.streamboard.tv/svn/oscam/trunk oscam-svn

cd oscam-svn

wget https://github.com/oscam-emu/oscam-emu/raw/master/oscam-emu.patch

patch -p0 < oscam-emu.patch

make config  >> add-ons  >> untick WITH_SOFTCAM  >> Ok  >> Save

make CONF_DIR=/etc/oscam USE_SSL=1 USE_LIBUSB=1

Hasil:
/root/oscam-svn/Distribution
oscam-1.20_svnXXXXX-XXX-aarch64-linux-gnu-ssl-libusb
Duplicate >> /bin/oscam

Folder oscam:
https://drive.google.com/open?id=16kXpSjSHoDp63bMyuk7Y4fI4mDKTKJ6Y

Run:
/bin/oscam &

Start On Boot
/etc/rc.local >> /bin/oscam &

Video :
Flash STB HG680P Armbian Linux (Dual Boot)                     https://youtu.be/X0Mwl7dAy9U
Flash STB B860H Android to Armbian and Armbian to Android      https://youtu.be/fzf6uXTZ8pw
Install Openmediavault STB HG680P Armbian Linux                https://youtu.be/3r7kKW8TXi0
Install Nginx MySQL phpMyAdmin Mikhmon OMV                     https://youtu.be/RuUOBpQrNVM
Install MPD Server STB Armbian Linux                           https://youtu.be/Ku8pCu1W-mU
Install Mikhmon dan Mikbotam                                   https://youtu.be/6kB6-ToJU2g
Building & Install OSCAM pada STB (HG860P/B860H) Armbian       https://youtu.be/HrG5JDidSRM 

Grup Facebook ARMBIAN LINUX STB HG680P B860H [ID]:
https://www.facebook.com/groups/447949046027700/

Regrads,
FuadSalim
fb.com/fuad.salim.drg
