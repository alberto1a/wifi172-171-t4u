# One driver for 3 wireless adaptors

WIFI 172-171-t4uv3

driver-kernel-version-files


Please see the driver followed
alberto1a/rtl8812AU_8821AU_linux forked from abperiasamy/rtl8812AU_8821AU_linux
I do my best and a lot of time testing drivers seriously and find not only one but still
severals work well as the followings, even moreover, some drivers can work for all 3 adapters, 
i.e. T4U ac1300 but also for dwa 172 and dwa 171 which are very popular in Taiwan or Mainland.

  All of working drivers are special thanks to The EDITORS IN GIBHUB.COM
  who helps to make them as formal drivers.

            How to install drivers for  TP-Link T4U ac1300 v3 USB3 in Linux system
     7 Drivers for TP-Link T4U ac1300 v3 USB3 (organized or created from June 27/2019) as previous one.

     The Installation of TP-link-T4U-AC1300-V3 USB3
      sudo apt-get install dkms -y
      sudo apt-get install build-essential linux-headers-generic linux-headers-`uname -r` -y
      sudo git clone   https://github.com/alberto1a/rtl8812AU_8821AU_linux.git
      cd  rtl8812au_8821au_linux 
      make clean
      make install -j8
      sudo modprobe cfg80211     (for t4u ac1300 v3)
      
      sudo make 
      sudo make install      
      sudo modprobe rtl8821ae     (for dwa172 and dwa172, the lines 27-29 modified)
                    
                  
   In such situations the drivers for adapters TP-Link T4U ac1300 v3 USB3 can be done successfully. 
   
   Some of drivers can work for 2 or 3 adapters, ( including D'Link DWA 172 and DWA 171)
            which makes users apply very easily and conviently. As the followings,
        
        by 1       alberto1a/How-to-install-TP-link-T4U-AC1300-V3
                  
           2      alberto1a/wifi172-171-t4u                                                      
                            (One driver for 3 wireless adapters)
           3       alberto1a/rtl8812AU_8821AU_linux forked from abperiasamy/rtl8812AU_8821AU_linux
                            (One driver for 3 wireless adapters)
                  
           4     wifi171-172-abperiasamy,  
                             (One driver for 2 wireless adapters)
           
           5        its-izhar/rtl88x2bu-driver
           6        cilynx/rtl88x2BU_WiFi_linux_v5.3.1_27678.20180430_COEX20180427-5959
                          (an excellent and best driver for T4u ac1300)
           7       Asus_USB-AC53_rtl8822bu 
                             (One driver for TP-link-T4U-AC1300-V3 adapters)
                  
        That's it for all friends need it in this free Linux world and the writer
             under the editor's request writing down my short experiences.
                     
                     
         It really can work for 3 different wireless adaptors,
             however, (I)    remember to forget (delete) the original connections 
             and      (III)  reboot the computer or 
                      (IV)   reset the router if necessary.
   
          It is usually not necessary if exchange between DWA 172 and DWA 171,
                 even (II)   reload the driver or reboot the computer.)
   
         But it needs to reload the driver when exchenge beetwee tp-link t4u ac1300 
             and  dwa 171 or dwa 172
    and reset the router or reboot the computer when it is dwa 171, but no need for dwa 172,   
              if necessary.
