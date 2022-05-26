#  2MoreF
> Calibration of CEM/AS3320 dual analog filter eurorack-modul.

## Preconditions<a name="preconditions"></a>
 Required or recommended tools are:

- 440Hz tone-reference (tuning-fork, fork oscillator etc.).
- Voltage meter.
- Frequency meter (if available).
- Eurorack for power (+12V/-12V) and keyboard-CV.
- 16pin Eurorack cable for modul-connection to the rack-bus.
- patchcables for modular synthesizers.

## Calibration<a name="calibration"></a>

**Table of Contents**

- [Offset-Adjustment](#offset_adjustment)
- [1V/Oct.-Adjustment](#1V_oct_adjustment)
- [Final check](#final_check)
- [License](#license)

> Board_B silk  
![Board_B silk overview](./pictures/2MoreF_BoardB_silk.png)  



### Offset-Adjustment<a name="offset_adjustment"></a>
> tbd.

### 1V/Oct.-Adjustment<a name="1V_oct_adjustment"></a>
> tbd.  

### Final check<a name="final_check"></a>
 Voltage measurements on Testpoint: TP1 and TP2.  

 The **'Res.'** (resonance)-potentiometers must be set to value:10 (**'CW'**, self oscillation).  
 Set **all other** potentiometers to **CCW** position.  
 >- connect voltage-meter between GND and TP1 or TP2.  

 The following table shows the measured voltages depending on the **'Frequency'**-potentiometer position.  

Poti-position | Frequency (Hz)       | measured voltage on TP1 or TP2 (mVolt)
--------------|----------------------|-----------------------------------
 min (CCW)    | less then 20 Hz      | 175 mVolt
 12 o'clock   | 440 Hz               |  84 mVolt
 max (CW)     | above 20 kHz         | -47 mVolt


## License<a name="license"></a>
> Hardware:cc by-nc-sa 4.0

