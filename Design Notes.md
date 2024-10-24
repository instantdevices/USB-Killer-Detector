<p align="center">
    <strong>DESIGN NOTES</strong>
</p>
<p><strong>Find notes below:</strong></p>
<ul>

<li>PCB is two-layer SMD.</strong></li>


<li>Design rules are Seeeds 2-layer standard rules.</li>

<li>Circuit has three sections, Micro USB charger, 5V boost converter and killer detector (including safety clamper).</li>

<li>
3-LEDs:
<ul>
<li>Power LED</li>
<li>Battery charger status LED</li>
<li>Killer detection LED</li>
</ul>
</li>

<li>Battery is 3.7V single cell Lithium Iron (1000mAh capacity). Charging current is 100mA (check schematic).</li>


<li>PCB size is mentioned in the given images. Basically ~3.6cmx6.2cm.</li>


<li>Mounting holes are 3mm.</li>


<li>The battery can be placed under the PCB. There is small rounded place to feed the battery wires from bottom side to top.</li>


<li>Some test points were added in case users need to check/debug circuit sections.</li>


<li>SJ1 jumper was added to reset the push button IC.</li>


<li>Additional external LED was added to the same Killer LED output. If users need to get out killer LED from the board to enclosure, skip board LED and R7 resistor and add R13 resistor. Then users can use EXT_LED header (2.54mm pitch) to drive external LED (LED will be standard 3mm, Vf=2.2V, If=20mA, these are approximates).</li>

<li>Added 4 fiducials for fab support.</li>

<li>S1 is the turn on/off button.</li>

<li>When a killer USB is detected, circuit will show the red LED output until removed. On low battery, red LED will turn on for the blink of an eye.</li>
</ul>
