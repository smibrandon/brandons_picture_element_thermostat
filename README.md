# Picture Element Thermostat

<img src="https://raw.githubusercontent.com/smibrandon/brandons_picture_element_thermostat/main/4_therms.PNG">

First and foremost, this is rough, I know. I'm sure there's a simpler way, and I'm all for suggestions. That all said, it works wonderfully on my tablet display.

This will show your thermostat's setting and state. I.E.: blue outlined for cooling set and orange outlined for heating set. When actively cooling or heating, it will be shaded in (like the two top examples). If it is set to off, it will be gray outlined.

1.  The items in `configuration.yaml` and `scripts.yaml` have to be added to the respective files. The `configuration.yaml` contains a few template sensors that the `picture_element` will read.
2.  Copy the `images` folder (including the images folder, itself) to your `www` folder.
3.  Create a new manual lovelace card and paste the contents of `Therm_card.yaml` in it.

This will have to be duplicated and modified for any additional thermostats added. So, with that said, I recommend coming up with a less-generic naming convention I used in this demonstration for the following entities:
    `sensor.visdisplay_state`
    `sensor.visdisplay_tempact`
    `sensor.visdisplay_tempset`
    `script.decreasetemp`
    `script.increasetemp`. I have mine to be the specific thermostate after the entity names above (`sensor.visdisplay_state_office`, for example)

Let me know your thoughts on this. It's my first project I've put out there, and I poured a lot of heart and soul in this, so I'd love to get feedback on it. 
