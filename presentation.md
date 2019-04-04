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

# Graphics APIs



---

# Crash Course in Computer Graphics

---

# Primitives

---

# With these three primitives, anything can be drawn

---

# Graphics APIs

---

# Common APIs

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
