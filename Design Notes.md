<p align="center">
    <strong>Design Notes</strong>
</p>
<p align="center">
    <strong></strong>
</p>
<p>
    1. PCB is two-layer SMD.
</p>
<p>
    2. Design rules are Seeeds 2-layer standard rules.
</p>
<p>
    3. Circuit has three sections, Micro USB charger, 5V boost converter and
    killer detector (including safety clamper).
</p>
<p>
    4. 3-LEDs are there,
</p>
<p>
    - Power LED
</p>
<p>
    - Battery charger status LED
</p>
<p>
    - Killer detection LED
</p>
<p>
    5. Battery is 3.7V single cell Lithium Iron (1000mAh capacity). Charging
    current is 100mA (check schematic).
</p>
<p>
    6. PCB size is mentioned in the given images. Basically ~3.6cmx6.2cm
</p>
<p>
    7. Mounting holes are 3mm
</p>
<p>
    8. The battery can be placed under the PCB. There is small rounded place to
    feed the battery wires from bottom side to top.
</p>
<p>
    9. Some test points were added in case users need to check/debug circuit
    sections.
</p>
<p>
    10. SJ1 jumper was added to reset the push button IC.
</p>
<p>
    11. Additional external LED was added to the same Killer LED output. If
    users need to get out killer LED from the board to enclosure, skip board
    LED and R7 resistor and add R13 resistor. Then users can use EXT_LED header
    (2.54mm pitch) to drive external LED (LED will be standard 3mm, Vf=2.2V,
    If=20mA, these are approximates)
</p>
<p>
    12. Added 4 fiducials for fab support.
</p>
<p>
    13. S1 is the turn on/off button.
</p>
<p>
    14. When a killer USB is detected, circuit will show the red LED output
    until removed. On low battery, red LED will turn on for the blink of an
    eye.
</p>
