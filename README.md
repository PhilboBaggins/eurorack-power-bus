# Eurorack Power Bus

<img align="right" src="./PlaceholderImage.png">

.....

## PCB design files

This board was designed using the [Upverter](https://upverter.com) web service.

The schematic, board layout and bill of materials can be viewed [here](https://upverter.com/Trebuchetindustries/c8ae200d804062f1/Eurorack-Power-Bus/). Exports from Upverter are available in a subdirectory.

The bill of materials lists specific a part number for the 3 LEDs but really any old 3mm through hole (radial) LED should work.

## Design calculations

### LEDs

The 3 LEDs indicate the presence of the 3 powers rails (+12V, -12V, +5V). They don't indicate that the power supply is behaving itself or that the power rail has the right voltage. LED brightness is controlled by the resistor next to each LED, recommended values:

* +12 volt rail: 5k ohms
* -12 volt rail: 5k ohms
*  +5 volt rail: 1.5k ohms

These resistances were calculated using the [design-calcs.ipynb](./design-calcs.ipynb) Jupyter Notebook. They were done with the following assumptions:

* Use an LED like this https://www.sparkfun.com/products/533
* Assume 2 volt DC forward drop for all LEDs
* Don't want the LEDs to be especially bright or use much current, 10 mA per LED will be fine
* Resistor values can be changed to increase or decrease brightness

## Mechanical

........

## Licence

Copyright © 2017, 2019 Phil Baldwin

This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0).

You should have received a copy of the license along with this work. If not, see <https://creativecommons.org/licenses/by-nc-sa/4.0/>.
