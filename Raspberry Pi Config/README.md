# Raspberry Pi files

This tree contains the config files I added and changed to make a Raspbian desktop install on a Raspberry 3 B work the way I wanted it to:

* A WiFi access point (with no internet access!) - the tablets and XR 18 hook up to this
* A DHCP server - obviously!
* A startup of a virtual VNC server when the WiFi network comes up - for debugging and admin
* A systel of "services" in the pi home folder that actually does the recording setup

I'll list prereqs and detailed instructions when I get time - but suffice to say you'll need 

* hostapd
* dnsmasq
* Real VNC Server
* sox (for recording - ALSA on it's own doesn't *quite* cut it because we need to amplify the incoming signals)

You'll also need to enable SSH access at boot

I'm hoping to slim this down so a full desktop install of Raspbian isn't necessary.
