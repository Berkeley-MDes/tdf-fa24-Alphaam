#### Overview:
For my homework, I worked on the following examples:
1. **FSR (Force Sensitive Resistor) to RGB LED Color Fader**
2. **Button to LED Pulse Rate Control**
3. **Basic Button Send-on-Change**

My overarching goal was to develop an understanding of how to manage inputs from physical components and translate them into responsive, real-time outputs.


### Reflections:

1. **FSR to RGB LED Color Fader**:
   - The project allowed me to explore how pressure applied to the FSR could dynamically control the color of an RGB LED. The FSR values were mapped to different RGB color combinations using a `switch()` statement and Pulse Width Modulation (PWM) to create smooth transitions between colors.
   - A key takeaway from this project was the effective use of analog inputs to continuously vary the LED output. I gained insights into managing color transitions with minimal delay, ensuring the color change was smooth and visually appealing.
   - I learned how to process sensor input through the Particle Device OS and output the data to actuate changes in the RGB LED using the `setTarget()` function to adjust the PWM values.

2. **Button to LED Pulse Rate Control**:
   - This project focused on using a button press to alter the flashing rate of an LED. Every button press would reduce the pulse rate, making the LED blink faster until a threshold was reached, at which point the rate would reset.
   - The major learning here was how to implement `attachInterrupt()` to handle button presses in real time, independent of the main program loop. This approach ensured that button presses were recognized immediately and the LED responded accordingly, even during delays in the loop.
   - Using interrupts also introduced me to the concept of handling multiple events within a microcontroller system and reacting to them without affecting other ongoing operations.

3. **Basic Button Send-on-Change**:
   - The goal of this project was to send button state changes to the Particle cloud only when the button's state actually changed, instead of constantly updating. This was managed within the `loop()` function, and only the first press or release event triggered a cloud update, ensuring that the system avoided spamming the cloud with redundant information.
   - Key insights from this project included the importance of managing data flow between hardware and cloud-based systems, and how to optimize communication using the `Particle.publish()` function to update the cloud efficiently.
   - A challenge was configuring the cloud connection and ensuring the button’s state changes were properly captured and reflected on the Particle cloud, which led me to explore Particle cloud tools and debug the connection.


### Challenges:

1. **Visual Studio Code Issues**:
   - Throughout all projects, I was unable to use the Visual Studio Code desktop app due to an error that consistently ended with "*... in archive is not an object.*" This prevented me from compiling code and flashing it directly from Visual Studio. As a workaround, I switched to using the Particle Web IDE, which allowed me to upload the code but limited my ability to debug and manage the projects as effectively as the desktop app would have. 
     - *(Screenshots of the error to be added here)*

2. **FSR to RGB LED**:
   - A challenge in this project was adjusting the sensor sensitivity so that the RGB LED responded appropriately to varying pressure levels. It took multiple iterations to fine-tune the ranges for the FSR, ensuring that light pressure caused subtle changes and harder presses yielded more vibrant colors.

3. **Button to LED Pulse Rate**:
   - Another challenge was managing the timing of the LED's pulse rate. The button presses had to result in significant, visible changes to the blink speed without making the transitions too abrupt. The use of interrupts was critical to addressing this, as it allowed the button press to be detected immediately and adjust the pulse rate smoothly.

4. **Button Send-on-Change**:
   - Initially, I struggled with establishing a reliable connection between the Photon 2 and the Particle cloud. Enabling `SYSTEM_THREAD(ENABLED)` was necessary to ensure that the microcontroller could connect to the cloud in the background while processing button inputs. I also had to carefully manage the frequency of cloud updates to avoid spamming the system with unnecessary data.


### Speculations:

1. **Future of the Projects**:
   - These projects can be expanded in multiple ways. For the **FSR to RGB LED**, adding additional sensors (e.g., temperature, light sensors) could allow for more complex interactions, where environmental conditions could also affect the LED’s color.
   - For the **Button to LED Pulse Rate**, adding more buttons to control other parameters, such as brightness or introducing new visual patterns, could make the system more interactive and dynamic. This could be extended to control multiple LEDs or devices.
   - For the **Button Send-on-Change**, integrating this system with other cloud-based platforms could enable real-time notifications or logging of button presses, making it useful for applications like remote monitoring or triggering actions in a home automation system.

2. **Machine Learning Potential**:
   - Each project could benefit from integrating machine learning, allowing the system to learn user patterns and optimize responses based on repeated interactions. For example, in the **Button to LED Pulse Rate** project, the system could learn preferred flashing rates based on how often the button is pressed at certain intervals. Similarly, the **FSR to RGB LED** could adapt the sensitivity to user behavior, making the system more responsive over time.

3. **IoT Ecosystem Integration**:
   - Combining the projects into a larger ecosystem could yield a responsive, interactive environment where multiple inputs affect various outputs. For instance, a button could control multiple RGB LEDs, each with different behaviors based on FSR inputs or cloud-triggered events. The potential for this kind of integration is vast in smart home or interactive installation scenarios.


### Project Documentation:

#### Circuit Assembly and Code:
Each project required precise circuit assembly to ensure smooth communication between the Photon 2, the input devices (FSR, buttons), and the outputs (LEDs). Below are images, videos, and sketches to document the steps taken for each project:

1. **FSR to RGB LED**:  
   *(Space for image of circuit, Fritzing diagram, and video)*  
   
   - The code reads the FSR input and assigns RGB color values based on pressure. The `setTarget()` function ensures smooth transitions between colors.
   
2. **Button to LED Pulse Rate**:  
   *(Space for image of circuit, Fritzing diagram, and video)*  
   
   - The button press modifies the LED pulse rate using an interrupt to detect real-time input and adjust the blink rate.
   
3. **Basic Button Send-on-Change**:  
   *(Space for image of circuit, Fritzing diagram, and video)*  
   
   - The button state is sent to the Particle cloud when a change is detected, ensuring minimal data transmission.

#### Error Screenshots:  
*(Space for screenshots of the Visual Studio Code error with the " ... in archive is not an object" message)*


### Future Directions:
- I plan to explore integrating additional sensors and actuators into these projects to create more complex, responsive systems. Expanding the **FSR to RGB LED** project to include other inputs or outputs would make the system more interactive.
- For the **Button to LED Pulse Rate** project, connecting the system to the cloud could enable remote control or monitoring of the LED’s behavior, opening possibilities for real-time interactions in IoT settings.
