### Progress Report for Monochrome 1.3" 128x64 OLED Graphic Display - STEMMA QT / Qwiic Project

---

#### Overview:
For this assignment, I experimented with the **Monochrome 1.3" 128x64 OLED Graphic Display - STEMMA QT / Qwiic** and integrated it with a Photon 2 microcontroller and a potentiometer. The project was built to display the potentiometer's value on the OLED screen. This experimentation serves as a foundation for a future project (Project 2, as described in the syllabus), where I plan to further incorporate the display and sensors for more advanced output.

---

### Reflections:

I began by soldering the STEMMA QT interface board, following the provided video instructions. The OLED display was connected to the Photon 2 via the I2C interface, allowing me to send data from the potentiometer to the display. Using Visual Studio Code and the Particle Workbench, I flashed the firmware to the Photon 2, and I was able to successfully display the potentiometer’s analog values in real time on the OLED screen.

One of the important learning experiences in this project was understanding how to interface external components like the OLED display with the Photon 2. The use of the I2C protocol to communicate between devices was relatively straightforward after setting up the necessary libraries in Visual Studio Code.

- I mapped the potentiometer values (ranging from 0 to 4095) using the `map()` function to an appropriate display format for the OLED. This allowed me to visualize how the values change as I rotate the potentiometer.
- The serial monitor provided insight into the raw potentiometer values, which were noisy at times. I experimented with the `constrain()` function to limit the range of values displayed on the OLED screen, ensuring the output remained stable and within the expected range.

---

### Challenges:

1. **Noise in Potentiometer Values**:
   - Initially, the values from the potentiometer were somewhat noisy, fluctuating more than expected. To address this, I used the `constrain()` function to limit the displayed values and smooth out the output, which improved the clarity of the data on the OLED.
   - Additionally, I considered implementing a basic moving average filter to smooth out the values further, but the `constrain()` function alone proved sufficient for this experiment.

2. **Feasibility of Mapping to Other Processes**:
   - I experimented with mapping the potentiometer values to other processes within the firmware code. For example, I considered outputting these values to an LED’s brightness using PWM, but in this case, I focused on stabilizing the values displayed on the OLED. Moving forward, I plan to explore how these values can be used to control other outputs, such as LEDs or motors, as part of Project 2.

---

### Speculations:

1. **Future Use in Project 2**:
   - In Project 2, I plan to use this OLED display to show real-time sensor data, such as temperature or humidity, along with the potentiometer values. This would provide a visual interface for users interacting with the system. Mapping the potentiometer values to control other devices or processes, such as the brightness of LEDs, will also be an important next step in expanding the project.
   - Additionally, I could integrate the `Particle.publish()` and `Particle.subscribe()` functions to send sensor data to other devices or share it with collaborators in real-time, making the project more interactive.

2. **Smoothing Out Noisy Values**:
   - Moving forward, I might further experiment with techniques to smooth out the noisy data from sensors, possibly implementing a more sophisticated filtering method. Using a moving average or exponential smoothing could make the readings more stable, which would be particularly useful when displaying sensitive or fluctuating data.

---

### Design Considerations:

#### Circuit Design:
The OLED display was connected to the Photon 2 via the I2C interface, and the potentiometer was wired to one of the analog input pins on the Photon. The circuit was simple but effective in demonstrating how sensor data can be displayed visually.

*(Space for images of the wiring and working system)*

#### Software Considerations:
In terms of software design, the project heavily relied on the `map()` function to scale the potentiometer values to the display's requirements. I also used the serial monitor to log raw values for debugging and ensured that the values sent to the display were constrained using the `constrain()` function to keep them within an acceptable range.

For future use, I plan to integrate additional sensor data into the OLED display, potentially creating a dashboard-like interface for real-time monitoring.

---

### Project Documentation:

#### Circuit Assembly and Wiring:
The wiring for this project included:
- **OLED Display (Monochrome 128x64)**: Connected via I2C using the STEMMA QT connector to the Photon 2.
- **Potentiometer**: Connected to an analog input pin on the Photon 2 to measure the resistance values and display them on the OLED.

![](https://github.com/Berkeley-MDes/tdf-fa24-Alphaam/blob/main/Week%206/media/IMG_3651.JPG)

![](https://github.com/Berkeley-MDes/tdf-fa24-Alphaam/blob/main/Week%206/media/IMG_3652.JPG)
*Pictures of circuit assembly and wiring*

#### Code:
The code included reading the analog values from the potentiometer, using the `map()` and `constrain()` functions to ensure the values are within a usable range, and displaying the values on the OLED screen. The `Serial.println()` function was also used to output values to the serial monitor for debugging purposes.

---

### Future Directions:
- **Integrating Other Outputs**: I plan to experiment with mapping sensor values to other outputs such as controlling an LED’s brightness or activating other components, making the system more dynamic and responsive to user input.
- **Particle Cloud Integration**: Another direction is using `Particle.publish()` to share sensor data with other devices or cloud services, potentially allowing remote monitoring of real-time data.



