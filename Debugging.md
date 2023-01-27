<p align="center">
    <strong>Debugging</strong>
</p>
<p align="center">
    <strong></strong>
</p>
<p>
    Components D1 and D5 should not be hot. However, they can be hot when it
    suppresses a power surge but, without power surge, they should not get hot.
</p>
<p>
    This device has internal diodes only. Please note that one pin is left un
    connected (VBUS pin).
</p>
<p>
    If users incorrectly solder these components (D1 and D5) and that
    particular unwanted pin is connected to power rail mistakenly, then diodes
    should get hot.
</p>
<p>
    Other reason for the abnormal heat is due to soldering.
</p>
<p>
    If user inserted a USB Killer to device and components D1 and D5 got hot,
    then may be these components are already dead by now.
</p>
<p>
    If this is the case, please remove components and continue lecture.
</p>
<p>
    ------------------------------------------
</p>
<p>
    Next step is checking voltage of the main surge detector IC (NX20P0408).
</p>
<p>
    User should check any GND pin of the circuit with D8 diode’s pin (USB side
    pin). This should be nearly 5V.
</p>
<p>
    If it is not nearly 5V, user has to check boost converter output voltage.
    It is TP12 and GND (not in above schematic).
</p>
<p>
    Then user needs some small voltage (limited current) source which can feed
    into USB Bus (bench power supply may work if user adjusts the current
    limiter around 300mA-500mA).
</p>
<p>
    Slowly user needs to increase the voltage up to around 28V at USB Data pins
    and check whether the main detector is triggered or not.
</p>
<p>
    To see if main detector is triggered, please check TP4 and +5V line with
    your voltmeter. If a power surge is detected, then voltmeter should show a
    value of around +5V. If this happens, user can conclude that the main
    detector IC is working.
</p>
<p>
    ------------------------------------------
</p>
<p>
    If there are not around +5V in your voltmeter while checking TP4 and +5V
    line, then main surge detector IC (NX20P0408) is not working as it should.
</p>
<p>
    The above can be due to several reasons:
</p>
<p>
    - IC (NX20P0408) was not soldered correctly.
</p>
<p>
    - Components in wrong positions.
</p>
<p>
    - Components soldered incorrectly.
</p>
<p>
    - Not all components are on board.
</p>
<p>
    At this point, it is recommended try to fix any of the above issues or
    start from zero.
</p>
<p>
    ------------------------------------------
</p>
<p>
    However, if there were +5V in the voltmeter while checking TP4 and +5V,
    then also check the resistance of F1. It should be very low.
</p>
<p>
    F1 acts as a conductor for normal operation.
</p>
