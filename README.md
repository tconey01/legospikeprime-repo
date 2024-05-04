![LEGO_SPIKE_Prime (2)](https://github.com/tconey01/legospikeprime-repo/assets/119706185/57541aa3-a0eb-41f1-a89f-007c188684f1)

# Happy coding! 🚀🔧

## [The Fundamentals](TheFundamentals)
### New to LEGO SPIKE Prime? Start here:
#### Explore step-by-step guides, from setting up your SPIKE Prime kit to writing your first lines of code.

## [Example Projects](ExampleProjects)
### Seeking Inspiration? Start here:
#### Your launchpad for exciting LEGO SPIKE Prime projects. Let the inspiration flow!

## **Quick Code Search**



| Color sensor                           | Code Snippet                           |
|---------------------------------|----------------------------------------|
| <img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/b604e2e9-c6cb-4ad3-827a-2c2206158ac3" width="500" height="400">
| 
  '''import runloop
    import color_sensor
    from hub import port
    import color'

    async def check_color():
       while True:  # This will create an infinite loop
          color_detected = color_sensor.color(port.B)
          if color_detected is not None:
              print(f"Color detected: {color_detected}")
              await runloop.sleep_ms(2000)
          else:
              print("No color detected")

          await runloop.sleep_ms(2000)  # wait for 4 seconds

    runloop.run(check_color())'''                                                    |
| Brief description of Example 1              | Explanation of the code in this example |
|                                             |                                         |

| Force sensor                          | Code Snippet                           |
|---------------------------------|----------------------------------------|
| <img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/95f8b808-f811-4a81-9804-e810ecf09ea1" width="500" height="400"> |       `from hub import color_sensor`              |
| Brief description of Example 1              | Explanation of the code in this example |
|                                             |                                         |

| Distance sensor                           | Code Snippet                           |
|---------------------------------|----------------------------------------|
| <img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/9d6b0a5b-4426-4bf6-abd2-97cd5b9b8e7f" width="500" height="400"> |       `from hub import color_sensor`              |
| Brief description of Example 1              | Explanation of the code in this example |
|                                             |                                         |

| Hub                           | Code Snippet                           |
|---------------------------------|----------------------------------------|
| <img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/d3353905-bfcd-4098-b764-7fb7994c7549" width="500" height="400"> |       `from hub import color_sensor`              |
| Brief description of Example 1              | Explanation of the code in this example |
|                                             |                                         |

| Motors                           | Code Snippet                           |
|---------------------------------|----------------------------------------|
| <img src="https://github.com/tconey01/legospikeprime-repo/assets/119706185/edbdae6f-0f32-4390-9b37-5ef9d69e2463" width="500" height="400"> |       `from hub import color_sensor`              |
| Brief description of Example 1              | Explanation of the code in this example |
|                                             |                                         |

                                           
