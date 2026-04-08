# VoRTis Media Gallery
[Back to Home](index.md)

This gallery showcases the core physical capabilities of the VoRTis solver, demonstrating how complex behaviors emerge from the grid-based physics without manual intervention.

---

## 1. Heavy cube drop under gravity
### **High-Velocity Impact** 
The real-time interaction of heavy cube dropping into the water pool under gravity. 

<video width="100%" autoplay loop muted playsinline style="border-radius: 8px;">
  <source src="assets/CubeDrop.mp4" type="video/mp4">
</video>

---

## 2. Wooden cube drop under gravity
### **Intrinsic Floating Dynamics** 
In VoRTis, buoyancy is not a "fake" force or a scripted volume. This clip shows the solver calculating upward force directly from the pressure displacement in the grid, allowing the cube to bob and settle naturally.

<video width="100%" autoplay loop muted playsinline style="border-radius: 8px;">
  <source src="assets/CubeDropBuoyancy.mp4" type="video/mp4">
</video>

---

## 3. Real-Time Navigation & Wakes
### **Interactive Vessel Control** 
A live look at two-way fluid-structure interaction (FSI). As the boat is driven through the domain, it generates realistic bow waves and trailing vortices that interact dynamically with the surrounding environment at interactive frame rates.

<video width="100%" autoplay loop muted playsinline style="border-radius: 8px;">
  <source src="assets/DriveBoat.mp4" type="video/mp4">
</video>

---

## 4. Kinematic Constraints & Rigid Body Coupling
### **Kinematic Interaction** 
This test demonstrates the solver's ability to handle kinematically driven objects. The fluid accurately responds to the forced motion of the geometry, showcasing the robustness of the pressure-velocity coupling.

<video width="100%" autoplay loop muted playsinline style="border-radius: 8px;">
  <source src="assets/KinematicCube.mp4" type="video/mp4">
</video>

---
[Return to Project Overview](index.md)
