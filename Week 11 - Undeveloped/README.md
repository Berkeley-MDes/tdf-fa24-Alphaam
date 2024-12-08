### Final Project Progress Report 

#### **Reflections**

**Conceptual Development:**
This week was heavily focused on ideation and concept refinement. I began with a critical examination of how culture, particularly in Tanzanian contexts, is often fluid, subjective, and misused for exclusionary purposes. Drawing on my personal experiences, I explored how socio-political powers shape cultural definitions to serve their narratives, often ignoring historical and communal nuances. A specific focus was placed on understanding the gap between the "culture" individuals perceive and the "culture" enforced by governing bodies.

To visualize this critique, I decided to use **Kitenge patterns** as a medium. Kitenge, as a fabric rich in cultural significance, became the perfect foundation for exploring and highlighting these inconsistencies. The patterns' vibrant colors, intricate repetitions, and rich textures provide an ideal backdrop for generative design experimentation.

**Research Process:**
I researched generative design tools and image analysis techniques to translate Kitenge patterns into a dynamic system that combines cultural critique with visual art. The primary tools and methods explored included:
- **p5.js**: A JavaScript library for generative art, which allows the creation of intricate, dynamic designs.
- **OpenCV with Python**: Used to analyze images and extract dominant colors and patterns from real Kitenge fabrics.
- **Google Colab**: Used to run Python scripts in a cloud environment to extract data from large images.

To ground my concept further, I analyzed **patterns in cultural enforcement**, specifically how governments use legal frameworks to enforce specific definitions of culture. I also examined how cultural exclusion manifests visually and symbolically, which shaped the visual direction of my project.

**Technical Trials:**
Initial experiments involved:
1. Testing OpenCV in Google Colab to extract dominant colors from Kitenge images.
   - Early attempts faced challenges with memory limitations when processing high-resolution images.
   - Adjustments included resizing images and sampling smaller pixel sets to optimize the clustering process.
2. Experimenting with **p5.js** for creating simple geometric shapes inspired by Kitenge patterns. I began by creating randomized shapes and integrating color palettes extracted from the reference images.

**Challenges:**
- Memory issues in Google Colab when analyzing high-resolution Kitenge images.
- Translating real-world patterns into generative designs while retaining authenticity and cultural depth.
- Balancing the conceptual critique with the aesthetic goals of the project.

---

#### **Speculations**

**Future Tool Direction:**
- Generative art tools like **p5.js** are rapidly evolving. I predict future integrations with machine learning tools, such as OpenCV, will allow for more seamless translation of real-world patterns into generative systems.
- OpenCV’s capabilities in pattern recognition may eventually extend beyond geometry and color to include more contextual metadata, such as historical and cultural relevance.

**Future Project Direction:**
- Next week, I plan to refine the visual representation of Kitenge patterns in p5.js, focusing on **repetition** and **shape integration**.
- I also plan to overlay symbolic data on top of the patterns, such as boundary thickness representing the rigidity of cultural enforcement by governing bodies.

---

#### **Images & Video**

1. **Kitenge Fabric Reference**:
   ![Kitenge Example](https://via.placeholder.com/800x400)  
   *(Reference image of Kitenge fabric used to inspire color palettes and pattern shapes.)*

2. **Initial OpenCV Color Extraction**:
   ![Color Extraction](https://via.placeholder.com/400x400)  
   *(Color palette extracted from the reference Kitenge fabric using K-Means clustering in OpenCV.)*

3. **Early p5.js Shape Rendering**:
   ![Shape Rendering](https://via.placeholder.com/800x400)  
   *(Screenshot showing early experiments with teardrop shapes inspired by Kitenge patterns in p5.js.)*

---

#### **Sketches, Drawings, and Diagrams**

1. **Concept Sketch of Cultural Critique Visualization**:
   - A rough hand-drawn sketch showing how colors and patterns will represent cultural perceptions and enforcement boundaries.

2. **System Workflow Diagram**:
   - Inputs: Reference Kitenge fabric, cultural enforcement data.
   - Process: Color extraction (OpenCV), pattern generation (p5.js), data mapping (interactive overlays).
   - Outputs: Generative art displayed interactively.

---

#### **Breadcrumb Trail**

- **Tools Used**:
  - OpenCV (image analysis and clustering).
  - p5.js (dynamic generative design).
  - Google Colab (Python environment for automation).
- **Resources Referenced**:
  - OpenCV documentation and tutorials on K-Means clustering.
  - Articles on cultural enforcement and visual storytelling.
  - Online repositories of Kitenge designs for inspiration.


