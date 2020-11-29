# This is my Home Assistant Configuration <img src="https://user-images.githubusercontent.com/50278221/99838601-a2804900-2b26-11eb-8e4b-d2cb986ca9b1.png" width="100" height="100" align="right">

</h1>
<p><strong>Be sure to <a href="#" title="star">⭐️</a> or <a href="#" title="fork">🔱</a> my repo if you find it useful! 🍻</strong></p>
<div align="center">
<h4> 
  <a href="https://www.smarthomemedic.com">
    Blog
  </a>
  <span> | </span>
  <a href="https://twitter.com/RasBe9244">
    My Twitter
  </a>
  <span> | </span>
   <a href="https://github.com/RamonBell/my_ha_setup/projects">
    Current Automation projects
  </a>
  <span> | </span>
<div align="center">
</a>
  </h4>

</div>
<p><font size="3">
This is my first Repo. I am trying to learn how to do this github thing. You will find more links to code and things for Home Assitant contained here.  I am constantly messing with my Home Assistant each day, sometimes messing it up. I will try to keep this updated as much as possible.  I use a configuration type called split configuration.  So my main configuration.yaml file is broken out into many different files located in the directories.  Once I load my config be sure to visit the package directory where the majority of the files exist. If interested in this method check out https://www.home-assistant.io/docs/configuration/packages/ </p>
<div align="center"><a name="menu"></a>

</div>
<p><font size="3">
I run my system on a Dell Optiplex 790 that is used from a doctor's office. I wiped it and put Promox on it as its operating system. I followed this repo and it took me twenty minutes to get it up and running: https://github.com/whiskerz007/proxmox_hassos_install. I moved away from cloud based devices and all my smart home deivces are run locally via MQTT.
  
# Table of Contents

- [Automations](#automations)
- [Sensors](#sensors)
- [Node Red](#nodered)

Here's the main components of my system:
| Amount | Item | Description |
|---|---|---|
|10 | Amazon Echo devices | How we talk to the house and notifications |
| 1 | Dell Optiplex | Runs Proxmox and Home Assistant |
| 1 | Sonoff Zigbee CC2531 USB Dongle|Zigbee Cordinator|
| 1 | Sonoff RF bridge | RF reciever (Tasmota Flashed) |
| 1 | Raspberry Pi4 | Use for Tuya convert, was my old HA operator |

<p align="right"><a href="#top" title="Back to top">🔝</a></p>

# Devices I use
Here's a run down of the devices that are used in my house.
* Switches:
  I use mostly physical switches in my house. I use a combination of Ayococr and Gosund switches flashed with Tasmota via Tuya Covert.
  
* Temperature and Humidity:
  I use Aquara Smart Home Temperature & Humidity Sesnors via Zigbee
  
* Motion Sensors:
  I use a combination of Aquara Zigbee, Sonoff RF and Kerui 433 Mhz RF motion detectors.
  
* Relays/switches
  I use Sonoff Basics flashed with Tasmota for lamps and other things that I wanted to make smart but not use a plug for. I have one Sonoff Basic ZBR3. Use it as a cordinator for my Zigbee system. Basically since it is always powered it helps with the mesh aspect of the Zigbee network.
  
* Plugs
  The plugs I use are a comibnation of Sonoff S26 and Sonoff S31 power monitoring plugs.
  
* RF Devices
  I use alot of RF devices throughout my house. The are very low power and battery operated. Here is yaml for the devices that I use. https://github.com/RamonBell/RF_devices/blob/main/yaml
<p align="right"><a href="#top" title="Back to top">🔝</a></p>

# Automations
 The majority of my automations, in one way or another, have to due with mine and my wife's unique work schedule and how things are turned on and off based on if we are home or  not or if we have a guest, or if we are on vacation, or if we are at work. Since my wife works nights and sleeps during the day, and I work four days a week very earily in the am, I use input booleans, location tracking and other methods to determine things that happen in the house. 
## Security Automations
   COMING SOON see https://github.com/RamonBell/my_ha_setup/projects/1
## Location Automations
   Presence Detection:
| Type | Links/Descritption | 
|---|---|
| NMAP | https://www.home-assistant.io/integrations/nmap_tracker| 
| MOBILE APP | https://www.home-assistant.io/integrations/mobile_app|
| MOTION DETECTORS | mix of RF and Zigbee 

## Football Automations
## System Automations
## Climate Automations
## Flood and Fire Automations
<p align="right"><a href="#top" title="Back to top">🔝</a></p>

# Nodered
 I use both Node Red and automations in HA. I feel that they can compliment each other greatly. I use Node red for more complicated automations with complex conditions. 1) I like the visualization of the flow. 2) I suck at Yaml and unless I can use the UI the automation, or steal someone else's code, it will fail. Here is a link for my Node Red flows: https://github.com/RamonBell/my_ha_setup/blob/main/nodered%20flows

<p align="right"><a href="#top" title="Back to top">🔝</a></p>

# Sensors
 I use alot of sensors that make decisions for my home automations
 * Workday https://www.home-assistant.io/integrations/workday/
 * Time/Date https://www.home-assistant.io/integrations/time_date/
 * Min/Max https://www.home-assistant.io/integrations/min_max/
 * Current Version https://www.home-assistant.io/integrations/version/
 * Comand Line https://www.home-assistant.io/integrations/sensor.command_line/#monitoring-failed-login-attempts-on-home-assistant
 * System Monitor https://www.home-assistant.io/integrations/systemmonitor/
 
 
 <p align="right"><a href="#top" title="Back to top">🔝</a></p>
 
Thank you for all visiting. Hit me up on my social outlets. If you want to contirbute feel free 🍻

<p align="right"><a href="#top" title="Back to top">🔝</a></p>

<p align="center"><strong>Don't forget to <a href="#" title="star">⭐️</a> or <a href="#" title="fork">🔱</a> this repo! 🍻</strong></p>


 

 


