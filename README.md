# HomeAssistant Dashboard Project

With my interest in smart home technology and energy conservation, I have added a multitiude of sensors around the house to monitor energy usage and wanted to create
an easy way to see that information in a usable way.

<a href="Video Demo of Dashboards" target="_blank"><img style="margin: 10px" src="https://russellventura.co.uk/wp-content/uploads/2022/11/HomeAssistant-Dashboards.mp4" alt="Demo Dashboard"  /></a>

I created 3 dashboards

#### Kitchen Dashboard

<a href="#" target="_blank"><img style="margin: 10px" src="https://russellventura.co.uk/wp-content/uploads/2022/11/KD.jpg" alt="Kitchen Dashboard"  /></a>  

This was the most complicated and most interactive of the dashboards.

Elements include:
Tumble Dryer toggle to on and off state - when on it shows live energy usage and a count down timer to turn off the smart plug when cycle complete
Washing Machine toggle to on and off state - when on it shows live energy usage and a count down timer to turn off the smart plug when cycle complete
Dish Washer toggle to on and off state - when on it shows live energy usage and a count down timer to turn off the smart plug when cycle complete

I have 18 lights in my kitchen, and used to turn them all on when using the room - this dashboard allows me to select the light or lights I want on
when performing a given task. Poppy light is selected for our dog so when she sleeps in the kitchen she has a light on at 5% brightness. The cooker light
is activated in the autumn / winter when we are preparing meals and cooking them, and the sink light is activated in the autumn / winter when we are cleaning up.

It has 2 additional buttons which link to the other dashboards - Energy Dashboard and Temperature Dashboard

Finally at the top, I have a temperature reading for the Kitchen.

#### GivEnergy Dashboard

<a href="#" target="_blank"><img style="margin: 10px" src="https://russellventura.co.uk/wp-content/uploads/2022/11/GivEnergy-Dashboard.jpg" alt="GivEnergy Dashboard"  /></a>  

We have recently had a solar & battery solution installed and wanted an easy way to check on its current status.

I created a dashboard in HA to show real time energy usage and status of the battery charge levels along with the temperature of the batteries and inverter.

I added some additional readings to help make decisions on when to run the appliances based on battery levels and solar production.

#### Temperature Sensors Dashboard

<a href="#" target="_blank"><img style="margin: 10px" src="https://russellventura.co.uk/wp-content/uploads/2022/11/Temperature-Dashboard.jpg" alt="Temperature Dashboard"  /></a>  

The temperature sensors used are SwitchBot thermostats which provide accurate temperature readings for each sensor.
Each sensor was placed in the relevant room and labelled

In order to access the Switchbot sensors in Home Assistant I had to hard code some configuration files and reboot my HA Raspberry Pi
They were then visible as entities within Home Assistant

I created a background image in Figma of the plan of the house (Ground Floor & First Floor)

I then created a Home Assistant dashboard and used the picture elemement card

I then added each sensor as a state-badge and positioned it to look good on a Google Nest Hub
I still have work to do to make it look good on desktop and mobile devices.

