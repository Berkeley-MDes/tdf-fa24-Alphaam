### TDF Final Project Progress Report 2

#### **Reflections**

**Refining the Kitenge Patterns:**
Building on the initial experiments from Week 1, this week focused on enhancing the authenticity and intricacy of the Kitenge-inspired patterns. The goal was to address challenges around the integration of shapes, texture, and randomness while ensuring the designs adhered to the **Key Features** identified earlier.

**Key Achievements:**
1. **Improving Shape Integration**:
   - Refined the teardrop shapes to ensure they appear more merged with the overall design rather than stacked on top.
   - Introduced subtle blending effects (`blendMode(OVERLAY)`) to create seamless transitions between overlapping shapes and the background.

2. **Adding Fabric Texture**:
   - Successfully implemented a more nuanced texture overlay, including:
     - **Noise points** to simulate the grainy look of printed fabric.
     - **Cross-hatch lines** to replicate the weave-like texture of Kitenge.
   - Adjusted the density and opacity of these textures to maintain subtlety without overpowering the design.

3. **Bleeding Effect for Black Lines**:
   - Enhanced the bleeding effect for black outlines by introducing slight perturbations in the stroke paths.
   - Added layers of opacity and varying stroke weights to make the lines feel more organic and ink-like.

**Challenges:**
- Balancing the vibrancy of colors with the texture overlay was tricky; early iterations looked overly muted or too noisy.
- Debugging shape placement randomness while maintaining the symmetry characteristic of Kitenge patterns.

**State of Work:**
By the end of the week, I had:
- A p5.js script capable of generating more authentic Kitenge-inspired patterns with improved texture and shape integration.
- A better understanding of how to balance the aesthetic elements of the design with the cultural critique embedded in the project.

---

#### **Speculations**

**Future Tool Direction:**
- Future developments in generative art tools like p5.js could include built-in texture libraries, enabling faster replication of complex material effects like fabric printing.
- AI models integrated with generative tools might soon allow direct style transfer from reference images, eliminating much of the manual experimentation currently required.

**Future Project Direction:**
- In Week 3, I plan to:
  1. Expand the range of shapes to include other Kitenge-inspired elements (e.g., stars, geometric grids).
  2. Begin testing interactivity features, allowing users to input cultural data (e.g., perceived values or enforcement levels) that will dynamically influence the patterns.

---

#### **Images & Video**

1. **Enhanced Teardrop Patterns**:
   ![Enhanced Teardrop Patterns](https://via.placeholder.com/800x400)  
   *(Teardrop shapes with improved blending and randomness, better mimicking Kitenge design.)*

2. **Texture Overlay with Cross-Hatch Lines**:
   ![Texture Overlay](https://via.placeholder.com/400x400)  
   *(Close-up of the texture overlay showing noise points and cross-hatch lines.)*

3. **Bleeding Black Lines**:
   ![Bleeding Black Lines](https://via.placeholder.com/400x400)  
   *(Example of the refined ink-bleeding effect applied to black outlines.)*

---

#### **Sketches, Drawings, and Diagrams**

1. **Updated System Workflow**:
   - Inputs: Extracted color palettes, cultural enforcement data.
   - Process:
     - Shape generation with integrated textures.
     - Mapping cultural data to visual attributes (e.g., boundary thickness).
   - Outputs: Refined Kitenge-inspired patterns.

2. **Diagram of Ink Bleeding Logic**:
   - A flowchart illustrating how perturbations and opacity layers were applied to create the bleeding effect.

---

#### **Breadcrumb Trail**

- **Tools Used**:
  - p5.js for shape generation and texture overlay.
  - Online tools like Image Color Picker for extracting additional reference colors.
- **Resources Referenced**:
  - Tutorials on `blendMode()` and noise generation in p5.js.
  - Close examination of Kitenge fabric for texture and pattern inspiration.

---


