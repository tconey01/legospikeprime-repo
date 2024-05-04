![LEGO_SPIKE_Prime (2)](https://github.com/tconey01/legospikeprime-repo/assets/119706185/57541aa3-a0eb-41f1-a89f-007c188684f1)

# Happy coding! 🚀🔧

## [The Fundamentals](TheFundamentals)
### New to LEGO SPIKE Prime? Start here:
#### Explore step-by-step guides, from setting up your SPIKE Prime kit to writing your first lines of code.

## [Example Projects](ExampleProjects)
### Seeking Inspiration? Start here:
#### Your launchpad for exciting LEGO SPIKE Prime projects. Let the inspiration flow!

## **Quick Code Search**



| Color sensor                    |
|:-------------------------------:|
| <p align="center"><img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/b604e2e9-c6cb-4ad3-827a-2c2206158ac3" width="500" height="400"></p> |    
| Code Description                |
|This code is a simple color detection program that continuously checks for colors using a color sensor connected to port B of a device. If a color is detected, it prints the color name; if no color is detected, it prints "No color detected", and it does this check every 4 seconds.    |


```python
import runloop 
import color_sensor
from hub import port
import color


async def check_color():
    while True:  # This will create an infinite loop
        color_detected = color_sensor.color(port.B)
        if color_detected is not None:
            print(f"Color detected: {color_detected}")
            await runloop.sleep_ms(2000)
        else:
            print("No color detected")

        await runloop.sleep_ms(2000)  # wait for 4 seconds

runloop.run(check_color())`


```

| Force sensor                    | 
|---------------------------------|
| <p align="center"><img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/95f8b808-f811-4a81-9804-e810ecf09ea1" width="500" height="400"></p> |  
|Code Description|
|This code is a simple force detection program that continuously checks for force using a force sensor connected to port A of a device. If force is detected, it prints the force value; if no force is detected, it prints “No force detected”, and it does this check in an infinite loop.    |

```python
import runloop
import force_sensor
from hub import port

async def read_force():
    while True:  
        force_detected = force_sensor.force(port.A)
        if force_detected is not None:
            print(f"\rForce detected: {force_detected}", end="")
        else:
            print("\rNo force detected", end="")

runloop.run(read_force())

```


| Distance sensor                 | 
|---------------------------------|
| <p align="center"><img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/9d6b0a5b-4426-4bf6-abd2-97cd5b9b8e7f" width="500" height="400"></p> |     
|Code Description|
|This code is a distance sensor program that continuously measures and displays the distance of an object from the sensor. If no object is detected, it clears the sensor reading and waits for a second before repeating the process.|

```python
import runloop
import distance_sensor
from hub import port

async def read_distance():
    while True:  
        distance = distance_sensor.distance(port.C)
        if distance is not None and distance >= 1:
            print(f"Distance: {distance} in")
            pixels = [100] * 4
            distance_sensor.show(port.C, pixels)
            await runloop.sleep_ms(1000)
        
        else:
            print("No object detected")
            distance_sensor.clear(port.C)  
            await runloop.sleep_ms(1000)

runloop.run(read_distance())

```


| Hub                             |
|---------------------------------|
| <p align="center"><img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/d3353905-bfcd-4098-b764-7fb7994c7549" width="500" height="400"></p> |     
|Code Description|
|This code displays different images on a device’s light matrix based on button presses. If the left button is pressed, it shows a happy image, and if the right button is pressed, it shows a sad image.    |

```python
from hub import light_matrix
from hub import button

while True:
    if button.pressed(button.LEFT):
        light_matrix.show_image(light_matrix.IMAGE_HAPPY)

    elif button.pressed(button.RIGHT):
        light_matrix.show_image(light_matrix.IMAGE_SAD)

```

| Motors                           | 
|--------------------------------- |
| <p align="center"><img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/1aa642f5-e84d-4d56-bea8-8f86f3b7eb92" width="500" height="400"></p> |
|Code Description|
|This is code       |

```python

code?

```


                                           
