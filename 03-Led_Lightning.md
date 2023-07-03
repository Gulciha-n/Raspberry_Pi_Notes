## Led Lightning with GPIO.RPi

```python
from RPi.GPIO import GPIO
import time

def blink(pin):
  GPIO.output(pin,GPIO.HIGH)
  time.sleep(0.5)
  GPIO.output(pin,GPIO.LOW)
  time.sleep(0.5)
  return

GPIO.setmode(GPIO.BOARD)
GPIO.setup(11,GPIO.OUT)

for i in range(0,50):
  blink(11)

GPIO.cleanup()
```

 Here's a step-by-step explanation of the code:

1. `from RPi.GPIO import GPIO` imports the `GPIO` module from the `RPi.GPIO` package. This module provides the functionality to control the  GPIO pins on the Raspberry Pi.
3. `import time` imports the `time` module, which is used for time-related operations such as delays.
4. `def blink(pin):` defines a function called `blink` that takes a parameter `pin`. This function will be responsible for turning the GPIO pin on and off to create a blinking effect.
6. `GPIO.output(pin, GPIO.HIGH)` sets the specified GPIO pin to a HIGH state, which turns it on.
7. `time.sleep(0.5)` pauses the program execution for 0.5 seconds, creating a delay.
8. `GPIO.output(pin, GPIO.LOW)` sets the GPIO pin to a LOW state, turning it off.
9. `time.sleep(0.5)` introduces another 0.5-second delay.
10. `return` statement ends the `blink` function.
11. `GPIO.setmode(GPIO.BOARD)` sets the pin numbering mode to BOARD, which refers to the physical pin numbers on the Raspberry Pi board.
12. `GPIO.setup(11, GPIO.OUT)` configures pin 11 as an output pin, indicating that it will be used to control an external device.
13. `for i in range(0, 50):` initiates a loop that will execute the following code 50 times.
14. `blink(11)` calls the `blink` function, passing pin 11 as an argument. This will turn the pin on and off with a delay, creating a blinking effect.
15. `GPIO.cleanup()` performs a clean-up of the GPIO resources, resetting the pins to their default state.

In summary, the code sets up pin 11 as an output pin, and then it repeatedly calls the `blink` function to make the pin blink on and off 50 times. 
Finally, it cleans up the GPIO resources.

Here's the screenshot:

![P1 py - Wokwi ESP32, STM32, Arduino Simulator - Google Chrome 7_3_2023 2_25_34 PM](https://github.com/Gulciha-n/Raspberry_Pi_Notes/assets/120305183/d0fe5778-5b16-46df-95d1-710aafc56e5b)

