# HomeAssistant Dashboard Project

With my interest in smart home technology and energy conservation, I have added a multitiude of sensors around the house to monitor energy usage and wanted to create
an easy way to see that information in a usable way.

I created 3 dashboards

## Kitchen Dashboard


## GivEnergy Dashboard



## Temperature Sensors Dashboard

The temperature sensors used are SwitchBot thermostats which provide accurate temperature readings for each sensor.
Each sensor was placed in the relevant room and labelled

In order to access the Switchbot sensors in Home Assistant I had to hard code some configuration files and reboot my HA Raspberry Pi
They were then visible as entities within Home Assistant

I created a background image in Figma of the plan of the house (Ground Floor & First Floor)

I then created a Home Assistant dashboard and used the picture elemement card

I then added each sensor as a state-badge and positioned it to look good on a Google Nest Hub
I still have work to do to make it look good on desktop and mobile devices.

