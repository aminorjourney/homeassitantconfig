These files are from my own Home Assistant install - you'll need to make your own tweaks, and I'm not responsible for any problems that come. 

You'll need to also add the relevant !include statements for each file. 

eg: template: !include <nameoftemplatefile>.yaml. 

You're also seeing INCOMPLETE configs here. I've removed PII and sensitive info, which is why I'm not including my Automations or my Scenes at this time (I need to go through and clean those up) 

I'll work to add missing helpers and integration as needed to make this all work, along with details of the various add-ons I've used. 

Just as a starter: 

* I'm using ESPHome for some of my sensors, specifically using two different Emporia Vue2 energy monitors running esphome. These are measuring power in to and out of the house. I will eventually share that YAML too ;)
* I'm using FordPass (https://github.com/itchannel/fordpass-ha) v1.7 (which still works!) to communicate with Ford's servers for my F150 Lightning status.
* I'm using the Onstar2MQTT integration (specifically the https://github.com/BigThunderSR/onstar2mqtt/ branch) to interact with my Bolt EV. It's recently been patched to work with the security updates/restrictions from GM.
* I'm using the JuicePassProxy project from https://github.com/JuiceRescue/juicepassproxy to connect two JuiceBoxes to my Home Assistant - I've made a few videos on that over at https://www.youtube.com/transportevolved/
* I ALSO have a Span Panel and am using the Span Panel integration here: https://github.com/SpanPanel It's available through HACS.
* You'll notice a lot of my config focuses on collating data - this is because I use the PowerFlow Plus card https://github.com/flixlix/power-flow-card-plus to represent my home energy consumption.
* I'm using the Enphase Envoy integration from Home Assistant: https://www.home-assistant.io/integrations/enphase_envoy. You'll notice I've removed my Enphae Envoy Serial number from the config files.
* For detecting charging station online status, I'm using Ping: https://www.home-assistant.io/integrations/ping
* For Acquanta smart heating, I'm using https://github.com/bmcclure/ha-aquanta
* And for NS Panel integration, I'm using the NSPanel Blueprint, but I may change that in the future ;) : https://github.com/Blackymas/NSPanel_HA_Blueprint
* I'm sure there's a bunch missing - please don't get frustrated if it's not there, you'll need to understand how to make sensors and meters to make sense of this ;) 





