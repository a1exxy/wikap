(admin)#show  platform

(admin)#show hw-module fpd location all

(admin)#install add tar disk0:ASR9K-px9-5.3.4_core.tar synchronous 

(admin)# show install summary

(admin)#install activate disk0:asr9k-px-5.3.4* synchronous 

(admin)#install commit

http://www.cisco.com/web/Cisco_IOS_XR_Software/pdf/ASR9K_Upgrade_Downgrade_Procedure_IOSXR_Rel_534.pdf