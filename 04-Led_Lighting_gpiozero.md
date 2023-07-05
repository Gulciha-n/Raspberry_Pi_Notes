# Led Lighting with gpiozero 

```python

from gpiozero import LED 
from time import sleep

led = LED("GPIO28") 

for i in range(0,10):
  led.on()
  sleep(0,5)
  
  led.off()
  sleep(0,5)
  
```
 Here's a step-by-step explanation of the code:

1. The first line imports the LED class from the gpiozero module and the sleep function from the time module.

2. The next line initializes an LED object named "led" and assigns it to GPIO pin 28.

3. The for loop is used to repeat the following code block 10 times.

4. Inside the loop, the `led.on()` method is called, which turns on the LED connected to the GPIO pin 28.

5. The `sleep(0.5)` function is called, which pauses the program execution for 0.5 seconds.

6. After the sleep period, the `led.off()` method is called, which turns off the LED.

7. Another `sleep(0.5)` function is called to pause the program execution for another 0.5 seconds.

8. The loop continues to the next iteration, repeating the on-off cycle of the LED.

9. Once the loop completes 10 iterations, the program exits.

In summary, this code turns on an LED connected to GPIO pin 28 for 0.5 seconds, then turns it off for another 0.5 seconds. This process is repeated 10 times.
