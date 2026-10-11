# graphics-lab

> Computer graphics experiments in C: rasterization, ray tracing, shading and rendering.

**Status:** Planned — roadmap only. No implementation has been claimed.

## Goal

Learn graphics algorithms in isolated, testable experiments and reuse mature ideas in sim-engine.

## Available / suggested hardware

Mac/PC. Start with a CPU renderer and image output; GPU experiments can come later.

## MVP (first demonstrable result)

1. Implement 3D vector/matrix transforms and perspective projection.
2. Rasterize a triangle to an image buffer and add a depth buffer.
3. Render a simple rotating 3D mesh and verify clipping, winding and interpolation.

## Next milestones

- [ ] Implement a basic ray tracer with spheres, reflections and shadows.
- [ ] Explore physically based materials, sampling and a small path tracer.
- [ ] Experiment with a GPU real-time rendering pipeline, shaders, shadow mapping and profiling.

## Skills to learn

- Coordinate transforms and geometric pipelines
- Triangle rasterization, clipping and Z-buffer
- Ray intersection and light transport
- Monte Carlo integration and real-time GPU rendering

## Connections to other repositories

- **sim-engine:** consumes reusable graphics modules; owns physics, simulation state and robot-world integration.
- **spatial-ui:** benefits from efficient camera, projection and interactive rendering.
- **cbrik:** optional home for tiny reusable math/utility code, not the whole renderer.

## Book study map

- **Fundamentals of Computer Graphics (5th ed.)** — Begin with geometry, transforms, rasterization, viewing and basic ray tracing.
- **Computer Graphics: Principles and Practice (3rd ed.)** — Use as a broad reference for graphics algorithms, mathematics and systems.
- **Real-Time Rendering (4th ed.)** — Use later for GPU pipelines, performance, shadows, materials and XR-relevant real-time techniques.
- **Physically Based Rendering: From Theory to Implementation (4th ed.)** — Use as an advanced reference for light transport, BSDFs, sampling and path tracing.

## What belongs here vs. sim-engine

| graphics-lab | sim-engine |
| --- | --- |
| Isolated rendering math and algorithms | Physical simulation, dynamics and robotics |
| Rasterizers, ray tracers, shaders and benchmarks | Simulated world, entities, joints and controls |
| Renderer demos and unit tests | Integrated demos that *use* the renderer |

Start with a CPU triangle rasterizer. You do **not** need to read all four books cover to cover before coding.

## Important scope note

Keep this a laboratory of rendering algorithms. Do not duplicate rigid-body simulation, collisions or robotics logic from sim-engine.

## Definition of done for MVP

- [ ] A reproducible demo or data output is committed.
- [ ] README explains how to run it.
- [ ] At least one validation result, plot, photo or screenshot is included.

## License

License to be selected before redistributing code.
