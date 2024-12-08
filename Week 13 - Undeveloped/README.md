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

1. **Expanded Shape Variety**:
   ![Expanded Patterns](https://via.placeholder.com/800x400)  
   *(A set of designs featuring new shapes, including stars and spirals, integrated into the Kitenge-inspired patterns.)*

2. **Interactive Interface Screenshot**:
   ![Interactive Prototype](https://via.placeholder.com/400x400)  
   *(Slider and dropdown menus allow users to adjust density and colors dynamically.)*

3. **Static Display Test**:
   ![Static Display](https://via.placeholder.com/800x400)  
   *(A mockup of the display system powered by a Particle Photon 2 microcontroller.)*

---

#### **Sketches, Drawings, and Diagrams**

1. **Final System Workflow**:
   - Inputs: User-selected cultural data, color palettes.
   - Process:
     - Shape generation in p5.js.
     - Integration of texture and boundary data.
     - Visualization output.
   - Outputs: Interactive generative art displayed digitally or via static installation.

2. **Diagram of Interactivity Features**:
   - A flowchart showing how user inputs are mapped to visual attributes like pattern density and color.

3. **Photon 2 Integration Plan**:
   - A diagram showing how the microcontroller and light sensor are connected to the display system.

---

#### **Breadcrumb Trail**

- **Tools Used**:
  - p5.js for pattern generation and interactivity.
  - Particle Photon 2 for display power management.
- **Resources Referenced**:
  - Tutorials on optimizing performance in p5.js.
  - Documentation for the Photon 2 microcontroller.

---
