### Weekly Progress Report - Week 1: OLED Display Integration & API Data Mapping

**Reflections:**
This week marked a significant milestone as I concentrated on the OLED display integration with the Photon 2, aiming to bring real-time data from the Tech for Palestine API directly onto the display. The primary objective was to create a seamless link between the API, which tracks the daily death toll in Gaza, and our OLED display, ensuring each update is promptly reflected. This involved establishing the data connection and configuring the Photon 2 to parse JSON data effectively, requiring a deep dive into both the Photon’s firmware and OLED display’s capabilities.

The process began with studying the Photon 2’s API handling protocols, particularly focusing on reading and structuring the JSON data for display. I encountered some initial issues related to the Photon’s handling of JSON objects; specifically, converting the API’s numerical data into a format compatible with the OLED’s display function was more complex than anticipated. I used Visual Studio Code to troubleshoot, gradually refining the code to ensure it accurately retrieved, parsed, and mapped the death count data.

This experience highlighted the nuances involved in interfacing with real-time data on compact screens like OLED. Beyond the technicalities, it emphasized the importance of optimizing data refresh rates to prevent overloading the Photon’s processing capabilities. Each attempt taught me about the Photon 2’s limitations and strengths, especially in managing JSON data and balancing display clarity with refresh rate.

**Speculations:**
Looking forward, optimizing the refresh rate for the OLED display will be essential to ensure that it doesn’t disrupt the experience. While rapid updates are ideal, there is a delicate balance to strike, as too-frequent refreshes could lead to performance issues, affecting user experience. Reflecting on how this project might evolve, I can envision applications that expand this concept beyond real-time counters, possibly integrating multiple data sources. As more developers integrate social justice data with interactive displays, I think there’s potential for real-time counters like this to serve as powerful installations in public spaces, provoking thought and conversation on humanitarian issues.

**Images & Video:**
1. **Screenshot**: Initial OLED display showing basic data render from the API.- incoming
2. **Photo**: Breadboard setup highlighting the OLED display and wiring connected to the Photon 2, annotated with connection points and descriptions.-incoming



