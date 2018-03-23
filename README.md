# Selks
Splunk Application for Selks IDS

The goal of this application is to provide a dashboard like the Kibana directly on Selks for Splunk using the log of the eve.json of the suricata of the appliance
This application provide you the same dashboard you can found on the appliance directly.

Selks project : https://github.com/StamusNetworks/SELKS

# Splunk - Installation

Connect to your splunk installation

create a index call "ids"

cd $HOME_SPLUNK/etc/apps

wget https://github.com/b4b857f6ee/Selks/archive/master.zip

unzip master.zip

 mv Selks-master/Selks ./
 
 mv Selks
 
 rm -rf Selks-master/
 
 chown splunk:splunk -R Selks   (only if your are using Splunk as splunk user and not root)
 
 restart splunk 
 
 # Selks Configuration
 
I am sending the logs with UF of the /var/log/suricata/eve.json

Check the splunk index to be sure.

index=ids


# Release Notes

