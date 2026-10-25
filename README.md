# Path Tracer `upcoming`

A physically based path tracer written from scratch in C++.

It renders realistic images by simulating how light bounces through a scene. The focus is performance: multithreaded rendering and a bounding volume hierarchy (BVH), with measured speedups.

## Planned features

- Diffuse, metal, glass, and emissive materials
- Antialiasing and depth of field
- Multithreaded tile rendering with per-pixel seeding, so output is identical at any thread count
- BVH acceleration with SAH splitting
- Triangle meshes loaded from OBJ files
- SDF shapes rendered by sphere tracing
- Scenes loaded from JSON files
- Command-line flags to render a single region of an image, for use by [Render Farm](https://github.com/vvoltaire/render-farm)

## Benchmarks

Coming soon: render times by thread count, and with and without the BVH.

## Tech stack

C++17, CMake, stb_image_write, tinyobjloader, GoogleTest

## References

Built starting from [Ray Tracing in One Weekend](https://raytracing.github.io/), extended with multithreading, BVH optimization, and SDF support.
