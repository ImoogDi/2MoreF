#  2MoreF
 Construction of CEM/AS3320 dual analog filter eurorack-modul.

**Table of Contents**

- [Preconditions](#preconditions)
- [Construction](#construction)
- [First Switchon](#firstswitchon)
- [License](#license)

## Preconditions<a name="preconditions"></a>

- All parts must be available for Board A and B (see BOM-files: [Board A](./../hw/2MoreF_BoardA_BOM.pdf) and [Board B](./../hw/2MoreF_BoardB_BOM.pdf)).
- The frontpanel is required for soldering Board A.

## Construction<a name="construction"></a>

>### Board A backside (start soldering here!) [backside-parts](./pictures/2MoreF_BoardA_parts_backside.png)

> start soldering parts on backside of Board A.  

>- place all SMD resistors and capacitors to the backside.
>- place all SMD diodes to the backside. Watch the rigth orientation and alignment.
>- place the three IC's to the backside. Watch the rigth orientation and alignment.
>- solder all parts on backside (reflow or by hand).
>- fit the 20-/16-position, 1 row headers to backside and solder them.
>- don't solder header K8 to backside (option for further extension)
>- at least Board A should look like this [BoardA_backside](./pictures/2MoreF_BoardA_backside.png)

>### Board A topside [topside-parts](./pictures/2MoreF_BoardA_parts_topside.png)

> continue soldering parts on topside of Board A.  

>- place all SMD capacitors to the topside.
>- solder all capacitors by hand.
>- **Don't solder yet any following parts before alignment to the frontpanel**
>- fit that snapin-potentiometers P1,P2,P3,P5,P6,P7,P8,P10 and P11 on PCB topside.
>- fit that snapin-potentiometers P4 and P9 on PCB topside.
>- fit that switches S1,S2 on PCB topside. Must be ON-Off-On type with three positions.
>- fit that switch S4 on PCB topside. Must be ON-On type with two positions.
>- fit that switch S3 on PCB topside. Must be ON-On type with two positions.
>- fit all eleven jacks on PCB topside.  
>- place the **frontpanel** on all of the topside parts and **allign** them.  
>- check alignment and distance to the frontpanel, see: [alignment](./pictures/2MoreF_BoardA_FP_alignment.png)
>- use nuts for the jacks, switches and pots to fix that frontpanel to the PCB-parts.
>- now solder all parts on backside and make sure everything is still aligned.
>- take a final view on Board A and place the knops on potis P4 and P9.
>- at least Board A with mounted frontpanel should look like this: [Frontpanel with BoardA](./pictures/2MoreF_Modul.png) 

>### Board B backside (start soldering here!) [backside-parts](./pictures/2MoreF_BoardB_parts_backside.png)

> start soldering parts on backside of Board B.  

>- place all SMD resistors and capacitors to the backside.
>- place the two IC's to the backside. Watch the rigth orientation and alignment.
>- solder all parts on backside (reflow or by hand).
>- fit the 20-/16-position, 1 row pin-headers to backside and solder them.
>- at least Board B backside should look like this: [BoardB backview](./pictures/2MoreF_BoardB_backside.png)


>### Board B topside [topside-parts](./pictures/2MoreF_BoardB_parts_topside.png)

> continue soldering parts on topside of Board B.  

>- place all SMD capacitors to the backside and solder them by hand.
>- place the two electrolytic capacitors to the topside and solder them.<br> (watch the correct orientation and aligment)
>- fit the DIL18 sockets to topside and solder them.<br> (watch the correct orientation)
>- fit the beads Filter1 and Filter2 to topside and solder them.
>- fit the 16 position, 2 row pin-header K1 to topside and solder it.<br> (watch correct alignment to the silk)
>- fit the 10 position, 2 row pin-header K9 to topsideand solder it.<br> (watch correct alignment to the silk)
>- fit the precision-potentiometers P1,P2,P3 and P4 to topside and solder them.<br> (watch correct alignment to the silk)
>- fit the eight styrene capacitores to topside and solder them.
>- at least Board B topside should look like this (with AS3320 in sockets): [BoardB topview](./pictures/2MoreF_BoardB_topside.png)

## First Switchon<a name="firstswitchon"></a>
 Preconditions:

- IC's:=AS3320 aren't yet fitted into the sockets on Board B.
- Board A and B are mounted together with there header and multipoint connectors.
- The frontpanel is placed on Board A and all nuts and knobs are mounted.
- 16pin buscabel is connected between eurorack-bus and the modul (watch the alignment of Pin1 := -12V).

 Action:

- Switch on the power on the eurorack-case.
- measure the voltage at socket X2, Pin14. Must be +12Volt.
- measure the voltage at socket X6, Pin14. Must be +12Volt.
- measure the voltage at socket X2, Pin13. round about -12Volt (without current-flow).
- measure the voltage at socket X6, Pin13. round about -12Volt (without current-flow).
- measure the voltage between testpoint TP1 and Ground GND.<br> repeat this measurement between testpoint TP2 and Ground GND.

 Result:

> measured voltages on TP1/TP2 depending on the **'Frequency'**-potentiometer position.  

<table>
<tr>
    <th>Poti-position</th>
    <th>measured voltage on TP1/TP2 (mVolt)</th>
</tr>
<tr>
    <td>min (CCW)</td>
    <td>less then:  +200 mVolt</td>
</tr>
<tr>
    <td>max (CW)</td>
    <td>higher then: -100 mVolt</td>
</tr>
</table>

> if this doesn't fit to above voltage-range the precision trimmers P1 | P2 (*offset*) have to be adjusted until that voltages are reached.


 Postconditions:

- IC's:=AS3320 are pushed into sockets on Board B. Watch the alignment of IC-pin1 to the socket.
- Calibration of the modul is required.



## License<a name="license"></a>
> Hardware:cc by-nc-sa 4.0

