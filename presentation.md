slidenumbers: true

# 3D Graphics Rendering with OpenGL
## Jerred Shepherd

^ Brief introduction about me

---

# Introduction

^ Computer graphics is something that all of us use every day, but most of us probably don't know much about it
^ Most of us won't write graphical programs running at such a low level, but it is cool to understand how things work

---

# What is graphics rendering?

^ Displays can be though of as a 2D matrix of pixels
^ Graphics rendering is how computers convey meaning on displays

---

# Where is graphics rendering used?
* Bootloaders
* Operating systems
* Video games
* Computer animation

^ Here are a few areas where graphics rendering is applied
^ Graphics rendering is used in very low-level places like text tendering for a bootloader, and high-level places like videos game and desktop applications

---

# Background

^ Why is graphics rendering special? What makes it its own field of CS?

---

# Graphics rendering requires a lot of computation
## :(

^ Graphics rendering involves positioning primitives in a 3D space and then drawing them on the screen
^ This requires a lot of math, which means our processors have a lot of calculation to do

---

# This computation can be done in parallel
## :)

^ It turns out that these calculations can be done easily in parallel

---

# CPUs are slow
## :(

^ Unfortunately CPUs are not fast enough
^ They are great for general computation, but aren't suited towards the task of computer graphics
^ They have too few cores and context switching is too slow

---

# GPUs are fast
## :)

^ GPUs were created as a coprocessor
^ They excel at floating-point operations, which is used heavily in computer graphics

---

# GPU Architecture

A diagram goes here

---

# Programming a GPU

^ Programming a CPU involves writing code, compiling it, and then executing a binary
^ Using a GPU is different
^ Instead of directly writing code, you use a API to communicate with the GPU
^ You can also write programs that execute on the GPU, but you still need to use APIs to load and execute the program
^ APIs exist for graphics programming, and for general computation
^ GPUs having become very popular for compute-heavy tasks, such as AI and data processing

---

# Graphics APIs
* OpenGL
* DirectX
* Vulkan
* Metal

^ Many graphics APIs exist
^ Which one you can use depends on your operating system and graphics card
^ OpenGL is a popular cross-platform API, and is supported on all modern consumer graphics cards

---

# Crash Course in Computer Graphics

^ Before we dig into OpenGL, it's important to understand some core concepts of computer graphics
^ These concepts will transfer over to any graphics API

---

# Primitives
* Points
* Lines
* Triangles

^ These are the three most important primivites in graphics rendering
^ With these primitives, you can draw anything you want

---

# Drawing a Complex Object

An image of a wireframe should go here

---

# Matrices

---

# Introduction to OpenGL

^ OpenGL is both a specification and a graphics API
^ The specification is defined by the Khronos Group
^ The API is implemented by the hardware manufacturer

---

# Where does OpenGL work?
* Language bindings exist for most languages

^ OpenGL is callable from most programming languages
^ OpenGL works one every major operating system, and with every major windowing system

---

# Java and OpenGL

^ Java has great support for OpenGL through a library called the Light-Weight Java Game Library (lwjgl)
^ Java and OpenGL is a great combination because it allows you to easily create cross-platform graphical applications
^ lwjgl has support for many other native libraries, some of which which we will use

---

# Getting Started with lwjgl

^ We will begin with creating a blank window on our desktop
^ This isn't particularly impressive, but it is a good place to start

---

# Creating a Window with GLFW

^ GLFW, or Graphics Library Framework, is a cross-platform library for creating windows and handling window events such as input
^ GLFW will create our window for us, and something called an OpenGL context
^ All of our drawing will occur within this OpenGL context

---

# Creating a Window with GLFW

```java
// Initialize GLFW
glfwInit();

// Create a new window with a given width, height, and title
long window = glfwCreateWindow(300, 300, "Hello World!", NULL, NULL);

// Set the newly created window at the current OpenGL context
glfwMakeContextCurrent(window);

// Show the window
glfwShowWindow(window);

// Creates OpenGL bindings using the current context
GL.createCapabilities();
```

---

# Preparing to Draw

^ Now we have a window where we can draw

---

# VAOs and VBOs

^ OpenGL stores vertices in vertex buffer objects
^ These buffers are then bound to vertex array objects
^ A VAO is then bound and drawn by OpenGL

---

# Creating a VBO

---

# Creating a VAO

---

# Binding a VBO to a VAO

---

# Binding a VAO and drawing it

---

# Our First Triangle

---

# Uniforms

---

# Indexed Rendering

---

# The Rendering Pipeline

---

# Shaders

---

# Textures

---

# References
* https://www.khronos.org/opengl/wiki/Language_bindings
* https://fgiesen.wordpress.com/2011/07/01/a-trip-through-the-graphics-pipeline-2011-part-1/

---

# Appendix #1: Clipping

---

# Appendix #2: Culling

---

# Appendix #3: Lighting

---

# Appendix #4: Matrices

---

# Appendix #5: Coordinate Spaces

---

# Appendix #6: w coordinate

---

# Appendix #7: Language bindings
* Ada
* C
* Common LISP
* C#
* C++
* Delphi
* Fortran
* Haskell
* Java
* Lua
* OCaml
* Perl
* Python
* Ruby
* Visual Basic
