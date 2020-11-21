![logo1](https://user-images.githubusercontent.com/50278221/99838601-a2804900-2b26-11eb-8e4b-d2cb986ca9b1.png)

<h1 align="center">
 My smart home setup
</h1>
<h4 align="center">Be sure to :star: this so you can get updates when I update my repo!</h4>
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
This is my first Repo. I am trying to learn how to do this github thing. You will find more links to code and things for Home Assitant contained in them.  I am constantly messing with my Home Assistant each day I will try to keep this updated as much as possible.  I use a configuration type called split configuration.  So my main configuration.yaml file is broken out into many different files located in the directories.  Once I load my config be sure to visit the package directory where all the YAML files exist.  </p>
<div align="center"><a name="menu"></a>

</div>
<p><font size="3">
I run my system on a Dell Optiplex 790 that is used from a doctor's office. I wiped it and put Promox on it as its operating system. Followed this repo and it took me twenty minutes to get it up and running: https://github.com/whiskerz007/proxmox_hassos_install. I moved away from cloud based devices and all my smart home deivces are run locally via MQTT.

Here's the main components of my system:
| Amount | Item | Description |
|---|---|---|
|10 | Amazon Echo devices | How we talk to the house and notifications |
| 1 | Dell Optiplex | Runs Proxmox and Home Assistant |
| 1 | Sonoff Zigbee CC2531 USB Dongle|Zigbee Cordinator|
| 1 | Sonoff RF bridge | RF reciever (Tasmota Flashed) |

Here are the majority of the devices that I use:
  Switches:
    I use mostly physical switches in my house. I use a combination of Ayococr and Gosund switches flashed with Tasmota via Tuya Covert.
  Temperature and Humidity:
    I use Aquara Smart Home Temperature & Humidity Sesnors via Zigbee
  Motion Sensors:
    I use a combination of Aquara Zigbee, Sonoff RF and Kerui 433 Mhz RF motion detectors.
  Relays/switches
    I use Sonoff Basics flashed with Tasmota for lamps and other things that I wanted to make smart but not use a plug for.
  Plugs
    The plugs I use are a comibnation of Sonoff S26 and Sonoff S31 power monitoring plugs.
 
    


</div>
<p><font size="3">
Mobile devices are the main way that we access our automation sysem.  They establish presence in the house and are the basis for many automations.  Are we home? Turn on Automations that do various things: lights, thermostat, alarm system.  Leave? Well do the oposite of being home. We use multiprong way of doing presense detection:
 
Presence Detection:
| Type | Links/Descritption | 
|---|---|
| NMAP | https://www.home-assistant.io/integrations/nmap_tracker| 
| MOBILE APP | https://www.home-assistant.io/integrations/mobile_app|
| MOTION DETECTORS | mix of RF and Zigbee 
 


