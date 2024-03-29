<!-- Please do not change this html logo with link -->
<a href="https://www.microchip.com" rel="nofollow"><img src="images/microchip.png" alt="MCHP" width="300"/></a>

# Basic Peripherals

This application uses the ADC to measure an analog input voltage, typically from a potmeter. It uses the sampled value to control the PWM duty cycle of an I/O pin, typically connected to a LED. The printf() will be redirected to USART to print status information, while the Timeout Driver schedules the timing of these operations. This results in a LED dimmer and printf() application.

## Related Documentation

- [ATtiny817 Device Page](https://www.microchip.com/wwwproducts/en/ATtiny817)

## Software Used

- [Atmel Studio](https://www.microchip.com/mplab/avr-support/atmel-studio-7) 7.0.2397 or later
- [ATtiny DFP](http://packs.download.atmel.com/) 1.6.316 or later
- AVR/GNU C Compiler (Built-in compiler) 5.4.0 or later


## Hardware Used

- [ATtiny817 Xplained Pro](https://www.microchip.com/DevelopmentTools/ProductDetails/attiny817-xpro)
- Micro-USB cable (Type-A/Micro-B)

## Setup

1. Connect ADC Channel 3 (PA3) to analog input voltage source, such as potmeter.

2. Connect PWM Channel 0 (PB0) to observable output, such as a LED.

## Operation

1. Connect the ATtiny817 Xplained Pro board to the PC using the USB cable.

2. Download the zip file or clone the example to get the source code.

3. Open the .atsln file with Atmel Studio.

4. Build the solution and program the device.

5. Open the EDBG COM-port in a terminal window to observe the printf() output.

6. Operate the analog input voltage source (e.g. potmeter) and observe the change in LED and printf() output.

## Conclusion

This code example has illustrated how to use basic peripherals of the ATtiny817 to create a LED dimmer and printf() application.
