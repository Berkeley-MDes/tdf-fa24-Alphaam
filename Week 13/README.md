### Final TDF Project Progress Report 3

#### **Reflections**

**Finalizing the Kitenge Patterns:**
This week, the focus was on refining and completing the core visual system for the Kitenge-inspired generative art project. With the groundwork from previous weeks, I concentrated on:
1. Expanding the variety of shapes and patterns while adhering to the **Key Features**:
   - Kitenge texture.
   - Shape position and size randomness.
   - Bleeding black lines.
   - Saturation and vibrancy of colors.
   - Seamless integration of all shapes.
2. Iterating on the texture and ink-bleeding effects to better mimic the organic imperfections found in traditional Kitenge fabric.

**Key Achievements:**
1. **Shape Diversity**:
   - Introduced new geometric shapes inspired by common Kitenge motifs, such as stars, spirals, and overlapping grids.
   - Layered these shapes with varying opacities and colors to create depth and richness.
   - Maintained randomness in size, position, and rotation to ensure an organic feel.

2. **Improved Texture**:
   - Adjusted the cross-hatch density and noise opacity for better balance across different designs.
   - Experimented with multi-layered textures to give the impression of a woven fabric.

3. **Interactive Prototype**:
   - Incorporated basic interactivity in p5.js, allowing users to:
     - Adjust the density of patterns via a slider.
     - Change the dominant color palette using dropdown menus.
     - Toggle the texture effect on and off for comparison.
   - This feedback-based addition was aimed at making the final product more engaging and dynamic.

4. **Static Display Integration**:
   - Planned the integration of the Particle Photon 2 microcontroller to manage the power for a static display.
   - Developed a basic test where the display powers off automatically when ambient light levels drop, conserving energy.

**Challenges:**
- Managing performance in p5.js as the number of shapes and texture layers increased. Early trials showed lag in rendering, which required optimizing the code by reducing unnecessary redraws and simplifying textures.
- Ensuring interactivity did not compromise the artistic integrity of the patterns.

**State of Work:**
- The p5.js script now produces a diverse range of vibrant, intricate patterns that effectively replicate Kitenge prints.
- A basic interactive interface allows customization, setting the stage for further refinement and testing with users.

---

#### **Speculations**

**Future Tool Direction:**
- Generative art systems like p5.js could benefit from libraries specifically designed for cultural and historical pattern replication, enabling faster and more accurate creation of designs like Kitenge.

**Future Project Direction:**
- The next step is to finalize the physical implementation, integrating the Particle Photon 2 with a light sensor for the static display.
- Plan to conduct user testing to refine the interactivity features, ensuring the final product effectively communicates the cultural critique.

---

#### **Images & Video**

**Realistic Kitenge Texture**:
   ![](https://github.com/Berkeley-MDes/tdf-fa24-Alphaam/blob/main/Week%2013/media/Screenshot%202024-12-05%20at%205.36.53%20PM.png)

   ![](https://github.com/Berkeley-MDes/tdf-fa24-Alphaam/blob/main/Week%2013/media/Screenshot%202024-12-06%20at%2011.27.54%20AM.png)


#### **Breadcrumb Trail**

- **Tools Used**:
  - p5.js for pattern generation and interactivity.
  - Particle Photon 2 for display power management.
- **Resources Referenced**:
  - Tutorials on optimizing performance in p5.js.
  - Documentation for the Photon 2 microcontroller.


