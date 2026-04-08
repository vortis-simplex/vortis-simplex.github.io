# Technical Architecture: VoRTis Solver
[Home](index.md) | [Media Gallery](gallery.md)

VoRTis is built on a custom high-performance framework designed to bridge the gap between offline scientific solvers and real-time game engines.

<video width="100%" autoplay loop muted playsinline style="border-radius: 8px;">
  <source src="assets/PlateRotation.mp4" type="video/mp4">
</video>

VoRTis is a real-time, high-performance, physically-accurate fluid simulator integrated with into Unreal Engine, delivering high-fidelity fluid behaviors (splashes, waves, vortices, etc.) and two-way fluid-structure coupling interaction at interactive frame rates. Unlike particle-based approaches, hydrodynamic forces and moments emerge intrinsically from the physics, enabling natural dynamics with arbitrary geometries without manual tuning. 

## Solver Methodology
Unlike the standard Niagara FLIP particles in Unreal Engine 5, VoRTis utilizes a **Grid-Based Continuum Solver**. This approach allows for:
* **Intrinsic Pressure Coupling:** Buoyancy and drag emerge naturally from the pressure-velocity solver rather than being approximated by heuristic forces.
* **Mass Conservation:** Strict adherence to the incompressibility constraint ($\nabla \cdot \mathbf{u} = 0$) ensures stable, physically accurate water surfaces.

## High-Performance Implementation
The solver is implemented as a standalone C++ module with deep integration into the Unreal Engine **Render Hardware Interface (RHI)**.

---
[View more example cases in the Gallery](gallery.md)
