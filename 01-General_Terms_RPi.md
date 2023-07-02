# Raspberry_Pi_Notes

### RX-TX: The RX and TX pins are the pins on Raspberry Pi used for data exchange.

The RX (Receive) and TX (Transmit) pins of Raspberry Pi are GPIO (general-purpose input/output) pins used for serial communication. 
The RX pin is used to transmit data from a device to Raspberry Pi, while the TX pin is used to transmit data from Raspberry Pi to another device.


### GPIO: General Purpose Input/Output

It represents the general-purpose input/output (GPIO) pins used to read or generate digital signals on a single-board computer like Raspberry Pi.There are 40 GPIO (general-purpose input/output) pins available on Raspberry Pi boards for various input and output operations.You can turn the light on and off, receive data from sensors, and interact with buttons.

### GND or VSS : 

#### "GND" = "Ground" , "VSS" = "Voltage Supply Ground"
The reference point, where the negative terminal or voltage source is connected, is commonly referred to as the ground. It typically represents the zero voltage level.

### GPIO.BOARD:
GPIO pin numbers are physically indicated to identify specific pins on a device. For example, in GPIO.BOARD mode, "Pin 5" refers to the physical pin number 5 on the board.

### GPIO.BCM:
It is a chip-specific numbering system. For example to access the 8th pin, you should write GPIO14.

### LIBRARIES:
```python
import RPi.GPIO as GPIO
```
```python
from gpiozero import LED
```

GPIO.HIGH:  Applies a high (3.3V) voltage to the GPIO pin.

GPIO.LOW:  Applies a low (0V) voltage to the GPIO pin.

GPIO.IN:  Sets the GPIO pin to input mode.

GPIO.OUT:  Sets the GPIO pin to output mode.

GPIO.setup(pin, mode):  Sets the operating mode of the specified pin (input or output).

GPIO.input(pin):  Reads the status of the specified pin (high or low).


 ### `GPIO.setmode(GPIO.BCM)`: To use GPIO pins with the BCM numbering scheme, we set it using the expression
 ### `GPIO.setup(led_pin, GPIO.OUT)`: To configure the `led_pin` as an output, we use the expression
 ### `GPIO.output(led_pin, GPIO.HIGH)`: To turn on the LED, we use the expression
 ### `GPIO.output(led_pin, GPIO.LOW)`: To turn off the LED, we use the expression
 ### `GPIO.cleanup()`:To clean up and release the GPIO pins, we use the expression

 

