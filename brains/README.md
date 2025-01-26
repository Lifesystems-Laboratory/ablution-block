# A section dedicated to the brains of the Ablution block


![alt text](https://raw.githubusercontent.com/Lifesystems-Laboratory/ablution-block/refs/heads/main/brains/smart_home.jpg)


Smart system to monitor & control ablution block is designed in a modular way. Main hub is connecting a lot of nodes. Each node is a seperate microcontroller that can work on it's own (monitoring and controlling one of the systems).

## Index of modules

* Main Hub (Home Assistant)
* Control dashboard (tablet or old PC)
* Air
  * air node 1 (indoor, display)  
  * air node 2 (shell, outdoor)
* Water
  * water node 1 (water tanks status)
  * water node 2 (pumps controls, display)
* Heating 
  * Heatpump (Tuya integration)
* Security
  * door node (smart lock)
  * camera node 1
  * camera node 2
* Power
  * 12v network node (in, out, levels)
  * 220v network node (in, out, levels)
* Light
  * indoor node (occupancy sensors, WLED)
  * outdoor node (motion sensors, security lights)
  


## Technology to make it happen: 

Each node is a ESP8266 or ESP32  with multiple sesnors and relay  https://esphome.io/ . Main hub is a Raspberry Pi running Home Assistant https://www.home-assistant.io/  Here is a good example of this kind of setup https://youtu.be/iufph4dF3YU

## General Setup (Current status to be updated)

We use Raspberry pi 4 (8gb Ram version) as a main computer for Home Assistant and followed installation instructions from here https://www.home-assistant.io/installation/raspberrypi 

As the wireless boards for ESPHome so far tested different versions of ESP8266: NodeMCU v1.1 and Wemos D1 mini, Wemos D1 mini pro. All boards seem to work as expected. They could be reprogrammed over wifi, after flashing them via USB connected directly to raspberry pi server. Followed different tutorials here from ESPHome and Home Assitant websites specific for the boards and sensors. 

Currently we just use power banks or usb power from raspberry but ideally each sensor cluster should have it's own local power sourse.  
We plan to make each wireles cluster of sensors individually powered with supercapacitors as a battery and solar panel or tiny water turbine as a generator. Each wireless board will be calibrated to take advantage of the 'deep sleep' power mode to only fully wake up when it needs to log data or when triggered by a sensor. 

Home Assistant is the great platform that will allow to collect and diplay data, together with ESPHome it will allow flexibility and scalability for the smart systems in Ablution Block and we will add constantly more sensors and controls as we experiment with different climate and water technologies.  

## User Experience 

Home Assistant provides many options to control settings and monitor all systems, in addition it will be possible to integrate any of the mainstream voice assistant. However we would like to make User Experience as intuitive and unobtrusive as possible using so called "calm technology" approach. 

"Calm technology" is a concept developed by Amber Case and Peter Morville in which technology is designed to blend seamlessly into the background of our lives, only becoming noticeable when it's needed. This can be achieved by using subtle cues, such as lighting or sounds, to indicate when an action is needed, and by keeping the interface simple and easy to use. In the context of our projects, this could mean designing interfaces for welfare units and Livesystems Laboratory that are intuitive and easy to use, and that minimize the need for user input. It could also mean using sensors and other technologies to monitor and control systems in the background, so that users are not constantly having to check and adjust settings. Additionally, it could involve designing the units to be visually unobtrusive and blend in with the surrounding environment.





