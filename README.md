# Hourglass
Hourglass is a custom PCB watch designed in KiCAD 7.0, to be funded by the Hack Club [OnBoard](https://github.com/hackclub/OnBoard/) grant, which allocates $100 for high schoolers to design and build their own custom PCBs.

## Revisions

### [Prototype:](./hourglass_prototype/) Concept test
> `Status: ❎ (SCRAPPED)`
<img src="./hourglass_prototype/hourglass_prototype_front.png" alt="reva front" width="300"/>
This is the original design I came up with when designing Hourglass, but due to size and wiring constraints, was scrapped. It utilizes two boards, one for controlling the watchface and the board which contains the face itself, which can be mixed and matched for upgradability or for a different means of displaying the time.

### [Revision A:](./hourglass_reva/) Working design iteration
> `Status: ✔️ (COMPLETE)`
<img src="./hourglass_reva/hourglass_reva_front.png" alt="reva front" width="300"/>
Revision A is the original design, based on the Atmel ATMega32u4 microcontroller. It features a RTC and 9DoF magnetometer-accelerometer to detect orientation, magnetic field strength and more to act as both a device for keeping time and sense when the wearer has raised the watchface to observe. In addition, a USB-C port can allow for interfacing directly to the Mega for uploading code and other functions.

### [Revision B:](./hourglass_revb/) Cost-effective design
> `Status: 🚧 (IN PROGRESS)`

Revision B is a easier, more affordable option. I'm working on this primarily because revision A is simply too expensive with all peripherals added in to have assembled via JLC's PCBA. It swaps the ATMega32 with an ATTiny84, the 9DoF magnetometer with a cheaper, magnetometer-only IC, and forgoes the need for dual-sided PCBA by having all SMD parts on one side.
