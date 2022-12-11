# HomeAssistant Dashboard Project


## UPDATE 11th December 2022 

I have continued to develop the dashboards and have added one (the humidity dashboard).

I have also migrated from casting to the google hub as it was proving unreliable and would either freeze, show a blank white screen or just disapear, so I purchased an Amazon Fire Tablet 8" HD and now use that device employing the <a href="https://www.fully-kiosk.com/" target="_blank"> Full Kiosk</a> solution. 

History:

With my interest in smart home technology and energy conservation, I have added a multitiude of sensors around the house to monitor energy usage and wanted to create
an easy way to see that information in a usable way.

I created 3 dashboards (now updated to 4 dashboards

## Kitchen Dashboard

<a href="#" target="_blank"><img style="margin: 10px" src="https://russellventura.co.uk/wp-content/uploads/2022/12/HA-Kitchen-Dashboard.png" alt="Kitchen Dashboard"  /></a>  

This was the most complicated and most interactive of the dashboards.

Elements include:
- <strong>Tumble Dryer</strong> toggle to on and off state | 
  By selecting the image of the Tumble Dryer this illuminates the image and activates the current (idle) counter preset to 1 hour. This is how long the cycle takes and then turns off the power once the countdown has expired saving energy by not leaving the dryer powered for ages. In addition is also provides live updates to how much power the appliance is using (shown in red) under Live Power Consumption.

- <strong>Washing Machine</strong> toggle to on and off state | 
  By selecting the image of the Washing Machine this illuminates the image and activates the current (idle) counter preset to 30 minutes. This is how long the cycle takes and then turns off the power once the countdown has expired saving energy by not leaving the washing machine powered. In addition is also provides live updates to how much power the appliance is using (shown in red) under Live Power Consumption.


- <strong>Dish Washer</strong> toggle to on and off state | 
  By selecting the image of the Dish Washer this illuminates the image and activates the current (idle) counter preset to 1 Hour. This is how long the cycle takes and then turns off the power once the countdown has expired saving energy by not leaving the washing machine powered. In addition is also provides live updates to how much power the appliance is using (shown in red) under Live Power Consumption.

I have 18 lights in my kitchen, and used to turn them all on when using the room - this dashboard allows me to select the light or lights I want on
when performing a given task. <strong>Poppy light</strong> is selected for our dog so when she sleeps in the kitchen she has a light on at 5% brightness. The <strong>cooker light</strong> is activated in the autumn / winter when we are preparing meals and cooking them, and the <strong>sink light</strong> is activated in the autumn / winter when we are cleaning up.

It has 2 additional buttons which link to the other dashboards - <strong>Energy</strong> Dashboard and <strong>Temperature</strong> Dashboard

Finally at the top, I have a temperature reading for the Kitchen along with a battery indicator to show the current state of the solar batteries charge level and then a clock showing the time and date.

<a href="https://github.com/russellventura/HomeAssistant/blob/main/Kitchen%20Dashboard" target="_blank"> View Kitchen Dashboard Code</a> 

## GivEnergy Dashboard

<a href="#" target="_blank"><img style="margin: 10px" src="https://russellventura.co.uk/wp-content/uploads/2022/12/HA-GivEnergy-Dashboard.png" alt="GivEnergy Dashboard"  /></a>  

We have recently had a GivEnergy solar & battery solution installed and wanted an easy way to check on its current status.

I created a dashboard in Home Assistant to show real time energy usage and status of the battery charge levels along with the temperature of the batteries and inverter.

#### Data from GivTCP API

- Inverter Serial Number
- Inverter Temperature
- Master Battery Charge Level
- Master Battery Temperature
- Master Battery Serial Number
- Slave Battery Charge Level
- Slave Battery Temperature
- Slave Battery Serial Number
- Excess Solar Production 
- Live Solar Generation
- Solar String 1 Solar Generation
- Solar String 2 Solar Generation 
- Total Solar Generation Today
- Total Solar Power Consumed Today
- Battery Power to Home
- Solar Power to Battery
- Batter Power to Grid
- House live power usage
- Live Power Usage (Updated from tesla-style-solar-power-card to Energy Distribution Card)

<a href="https://github.com/russellventura/HomeAssistant/blob/main/GivEnergy%20Dashboard" target="_blank"> View GivEnergy Dashboard Code</a> 

## Temperature Sensors Dashboard

<a href="#" target="_blank"><img style="margin: 10px" src="https://russellventura.co.uk/wp-content/uploads/2022/12/HA-Temperature-Dashboard.png" alt="Temperature Dashboard"  /></a>  

The temperature sensors used are <a href="https://www.amazon.co.uk/SwitchBot-Thermometer-Hygrometer-Temperature-Compatible/dp/B09JW6N72V" target="_blank"> Switchbot Thermometers</a> which provide accurate temperature readings for each sensor.
Each sensor was placed in the relevant room and labelled

In order to access the Switchbot sensors in Home Assistant I had to hard code some sensor configuration files and reboot my HA Raspberry Pi
They were then visible as entities within Home Assistant

I created a background image in Figma of the plan of the house (Ground Floor & First Floor)

I then created a Home Assistant dashboard and used the picture elemement card

I then added each sensor as a state-badge and positioned it to look good on an Amazon Fire Tablet 8" HD
Further development is required to create dashboards that look their best on all devices.

<strong>UPDATE:</strong> I have added a humidity icon to the top centre of the dashboard that links to the humidity dashboard

<a href="https://github.com/russellventura/HomeAssistant/blob/main/Temperature%20Dashboard" target="_blank"> View Temperature Dashboard Code</a> 

## Humidity Sensors Dashboard

<a href="#" target="_blank"><img style="margin: 10px" src="https://russellventura.co.uk/wp-content/uploads/2022/12/HA-Humidity-Dashboard.png" alt="Humidity Dashboard"  /></a>  

The humidity sensors used are <a href="https://www.amazon.co.uk/SwitchBot-Thermometer-Hygrometer-Temperature-Compatible/dp/B09JW6N72V" target="_blank"> Switchbot Thermometers</a> which provide accurate humidity readings for each sensor.
Each sensor was placed in the relevant room and labelled

In order to access the Switchbot sensors in Home Assistant I had to hard code some configuration files and reboot my HA Raspberry Pi
They were then visible as entities within Home Assistant

I created a background image in Figma of the plan of the house (Ground Floor & First Floor)

I then created a Home Assistant dashboard and used the picture elemement card

I then added each sensor as a state-badge and positioned it to look good on an Amazon Fire Tablet 8" HD
Further development is required to create dashboards that look their best on all devices.

<a href="https://github.com/russellventura/HomeAssistant/blob/main/Humidity%20Dashboard" target="_blank"> View Humidity Dashboard Code</a> 
