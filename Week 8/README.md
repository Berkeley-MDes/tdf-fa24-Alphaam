---

### Weekly Progress Report - Week 2: LED and FSR Setup for Symbolic Representation

**Reflections:**
This week’s focus was setting up and configuring the LED lights and Force Sensitive Resistor (FSR) to add symbolic and interactive layers to the Palestinian Death Counter. Given the importance of creating an emotionally impactful piece, we chose red and green LEDs to represent colors of the Palestinian flag, with the intent that their flickering would communicate the data updates in a subtle yet disturbing manner. My work involved coding the LED behavior to not only respond to the death count but also adjust dynamically based on the FSR readings, creating a more immersive experience for the viewer.

The integration of the FSR added complexity to this setup. My goal was to allow the LED brightness to increase or decrease based on how close someone is to the sensor, giving a sense of engagement as the numbers grow. I experimented with various sensitivity thresholds, adjusting the FSR’s response until it achieved a smooth yet noticeable change in brightness. This experimentation taught me a lot about force-sensitive technology, as even small variations in applied force significantly affected the LED’s output. This feedback loop was then calibrated to work seamlessly with the Photon 2, which required additional code to ensure the FSR and LED interactions were in sync with the API data.

Overall, these additions enhance the project’s symbolism, making it feel more alive. Each time the counter updates, the lights flicker—a visual disturbance that mirrors the growing death toll. This setup required multiple rounds of testing, as I calibrated the LED’s response to provide just the right amount of feedback, making it visually unsettling without overwhelming the OLED display’s information.

**Speculations:**
For the future, I’m excited by the possibility of adding more sensors or even expanding the symbolic elements. Integrating elements such as vibration motors or sound could further amplify the immersive quality, helping it become a poignant installation piece. With the rise of interactive data displays in raising awareness, I believe we are moving toward a future where technology like this is used as a tool for social consciousness in public installations and educational environments. The FSR and LEDs, in particular, have enormous potential in museum or gallery settings where viewers seek not only to understand information but to feel its emotional weight.

**Images & Video:**
1. **Video Clip**: This video clip shows the LED flickering in response to API data updates, capturing the effect of intermittent light patterns - incoming
2. **Photo**: Setup photo showing LED and FSR wiring, annotated with connection points to illustrate the integration with the Photon 2.- incoming



