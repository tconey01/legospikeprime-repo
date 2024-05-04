![LEGO_SPIKE_Prime (2)](https://github.com/tconey01/legospikeprime-repo/assets/119706185/57541aa3-a0eb-41f1-a89f-007c188684f1)

# Happy coding! 🚀🔧

## [The Fundamentals](TheFundamentals)
### New to LEGO SPIKE Prime? Start here:
#### Explore step-by-step guides, from setting up your SPIKE Prime kit to writing your first lines of code.

## [Example Projects](ExampleProjects)
### Seeking Inspiration? Start here:
#### Your launchpad for exciting LEGO SPIKE Prime projects. Let the inspiration flow!

## **Quick Code Search**



| Color sensor                    | Code Description                       |
|---------------------------------|----------------------------------------|
| <img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/b604e2e9-c6cb-4ad3-827a-2c2206158ac3" width="500" height="400"> |    This is code    |

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

| Force sensor                    | Code Description                       |
|---------------------------------|----------------------------------------|
| <img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/95f8b808-f811-4a81-9804-e810ecf09ea1" width="500" height="400"> |    This is code    |

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


| Distance sensor                 | Code Description                       |
|---------------------------------|----------------------------------------|
| <img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/9d6b0a5b-4426-4bf6-abd2-97cd5b9b8e7f" width="500" height="400"> |     This is code    |

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


| Hub                             | Code Description                       |
|---------------------------------|----------------------------------------|
| <img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/d3353905-bfcd-4098-b764-7fb7994c7549" width="500" height="400"> |      This is code    |

'''

'''

| Motors                           | Code Description                       |
|--------------------------------- |----------------------------------------|
| <img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/edbdae6f-0f32-4390-9b37-5ef9d69e2463" width="500" height="400"> |   This is code       |

'''

'''


                                           
