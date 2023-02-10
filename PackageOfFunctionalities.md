My idea is a open-source Sonoff POW R3 for AC-power energy meter based on a ESP32 S2 Mini.

I need help improving/reviewing my KiCAD design. I learnt electronics from Youtube vids.

The (incomplete) <a href="https://github.com/pappavis/StroomMeterACS712/tree/main#benodigheden" target="_blank">BOM</a> is;
- ESP32 S2 Mini
- HLK-PM01_220V AC-DC powersupply
- PCF8574A I2C expander
- SRD-03VDC-SL-C_Relay
- OLED1604 I2C
- ACS712ELCTR-05B-T power measurement
- A few pushbuttons, LEDs, resitors
- Screw terminals for AC-power in&out

Functionally;
- A user should connect 220V-wire from mains
- A status LED for indicating on/off state
- A status for when 220V is being measured
- Ability to (de)activate the relay, and therefore switch of power to anything connected to it


Technical;
- I'm using plug-in modules such as the OLED screen, ACS712, ESP32 S2 etc.
- Must all be on one circuitboard of <>10cm squared -- to save on PCB manufacturing cost.
- Using through hole components, though SMD are welcome wherever possible to save space.

My design is on my github page. I'll be writing the code for above in MicroPython

When you accept;
- Can you review it, improve, and fix my mistakes?
- If you accept the job, can we have a Whatsapp call once or twice to clear inconsistencies?

I'll upload the full design and manufacturing documentation onto my Github page.

let me know.. your rate to review my work?

regards,
Michiel.
