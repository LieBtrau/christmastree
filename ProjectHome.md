A printed circuit board (PCB) is made into the shape of a christmas tree.  On one side of the PCB, some LEDs are placed, which will gradually change color when power is applied to the circuit.
5V Power must be applied to the USB-mini connector.

# Project Inspiration #
![![](http://christmastree.googlecode.com/files/vector-christmas-tree-digital-circuit_small.jpg)](http://christmastree.googlecode.com/files/vector-christmas-tree-digital-circuit.jpg)

The main reason for starting this project was to find an original christmas card.

# Requirement specification #
  * Must be small enough to fit a standard envelope.
  * Must be powered from an easy to get power source
  * Preferably environmentally friendly
  * Power consumption must be lower than 0.5W.
  * Device must be able to survive in a tropical climate.
  * Device must be in the shape of a christmas tree.
  * There must be lights on that christmas tree of different colors.
  * Colors of the lights must change gradually, a fading effect.
  * Control logic should be kept out of sight as much as possible to avoid dragging away the attention from the fading lights.
  * Must be possible to hang up the device somewhere on a hook or a cord.
  * Must contain easy to get components.
  * Must not contain programmable logic.

# Technical realisation #
  * Device fits in a [shipping box](http://faisst-koffer.de/shipping-boxes.html).
  * Power source
    * No non-rechargeable batteries, because not environmentally friendly.
    * No rechargeable batteries, because the correct charger is not available everywhere.  Integrating a charger on the circuit would make it too expensive.
    * USB-power is selected.  USB-chargers are readily available to charge MP3-players, cell-phones, ...  These are available around the globe and are pretty cheap.  The user has to buy it, so it's always the correct power plug.
    * USB-mini connector is chosen instead of USB-B, because of the lower height.
    * Power consumption should be lower than 0.5W.  24LEDs are used that draw 15mA at an average.
  * The device will be tropicalized.
  * 24 RGB-LEDs are used.  Only two LEDs in each package are used.  All three combinations (red-green / red-blue / green-blue) occur eight times on the PCB.
  * The fading effect is created by XOR-ing the output of two oscillators with a slight difference in frequency.  The idea comes from [Elektor](http://www.seekic.com/blog/project_solutions/2011/08/18/Playful_Lights__Just_there_LEDs.html)
  * LEDs are placed on top side of the PCB, the other components are placed on the bottom side.
  * The christmas tree has a 3mm-hole on top for a cord.
  * All control is done with standard 74-series logic, some resistors and some capacitors.

## [Revision 0](https://code.google.com/p/christmastree/source/detail?r=0) ##
  * [Design data](http://christmastree.googlecode.com/files/BRD111111_0__.PDF)

![![](http://christmastree.googlecode.com/files/PCB_top_small.jpg)](http://christmastree.googlecode.com/files/PCB_big_top.jpg)
![![](http://christmastree.googlecode.com/files/PCB_small_bot.jpg)](http://christmastree.googlecode.com/files/PCB_big_bot.jpg)