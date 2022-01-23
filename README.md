# Biltemeas Babycam

A friend asked for help with this cam, the password under the cam does not work and in playstore there is alot of ppl that seems have the same problem.


![Screenshot](babycam.png)

Various pictures

![Screenshot](https://wuseman.nr1.nu/archive/babycam/0001.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0002.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0003.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0004.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0005.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0006.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0007.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0008.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0009.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0010.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0011.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0012.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0013.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0014.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0015.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0016.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0017.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0018.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0019.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0020.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0021.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0022.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0023.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0024.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0025.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0026.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0027.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0028.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0029.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0030.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0031.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0032.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0033.jpg)
![Screenshot](https://wuseman.nr1.nu/archive/babycam/0034.jpg)


#### Here you go: 


    Lets Hack: 

    Poweron your babycam
    Connect to the babycams wifi 
    Once connected, find ip to the cam:

    for ip in 192.168.1.{1..254}; do
        ping -c 1 -W 1 $ip | grep "64 bytes" &
    done
 
Connect to the webcam:

    telnet 192.168.1.X

    Login:      root
    Password:   root

    Create wpa_supplicant.conf

    cat << EOF > /mnt/sif/wpa_supplicant.conf
    ctrl_interface=/var/run/wpa_supplicant
    network={
    ssid="EDIT_THIS"
    psk="EDIT_THIS"
    scan_ssid=1
    key_mgmt=WPA-EAP WPA-PSK IEEE8021X NONE
    pairwise=TKIP CCMP
    group=CCMP TKIP WEP104 WEP40
    eap=TTLS PEAP TLS
    proto=WPA RSN
    frequency=2414
    scan_freq=2412
    }
    EOF

Then Reboot! 

    reboot

Now you will see the app in your biltemas shitty application 
    
Download app: https://play.google.com/store/apps/details?id=hk.biltema.com&hl=no&gl=US

#### Those cams are dangerous, really! They claim there is no cloud but that is really needed?

![Screenshot](babycam_mirroring.gif) 


#### Manuals


    https://www.biltema.se/BiltemaDocuments/Manuals/24-0433_man.pdf
