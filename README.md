# BARZOIUS

**`C++ enthusiast 🛠`**
                                                                    
Barzoius is just a nickname, my real name is Rareș.                            
Not much to say yet, I like C++, graphics and physics.                           
               
   <p align="left">
      <a href="https://www.linkedin.com/in/moisel-rares-936258268/">
       <img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" /> </a>
   
---
   ###  Things I am learning:
 <div style="display: flex; align-items: center;">
    <img alt="C++" width="45px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/cplusplus/cplusplus-original.svg" />
    <img alt="OpenGL" width="80px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/opengl/opengl-plain.svg" />
    <img alt="DirectX" width="95px" style="padding-right:10px;" src="https://upload.wikimedia.org/wikipedia/commons/7/7f/Microsoft-DirectX-Logo-wordmark.svg" />
</div>
<br><br><br>

## Framework Overview

<img src="GraphicsSandBox/Resources/ForREADME/diag2.png" alt="Framework Diagram" style="width:100%;">

- **Drawable**: A base class that contains a vector of shared pointers to `Bindable` objects, which represent GPU resources (Vertex Buffers, Index Buffers, Constant Buffers, Shaders, etc.).
- **Mesh**: Inherits from `Drawable` and represents a renderable object. It utilizes the `Drawable`'s bindables to define its rendering behavior.
- **Codex**: A resource management class that maintains a map of all created `Bindable` objects. When a `Mesh` requests a `Bindable`, the `Codex` checks if it already exists, allowing for resource reuse and avoiding redundant creation.
