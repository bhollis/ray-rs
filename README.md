# Rust Raytracer

[![Build Status](https://travis-ci.org/bhollis/ray-rs.svg?branch=master)](https://travis-ci.org/bhollis/ray-rs)

Back in college I made a C++ raytracer with photon mapping in a graphics class. This year I found the code again and got it running, then decided to rewrite it in Rust as a learning tool. Note that most of the original code was provided as a "starter kit" to me and isn't mine - I had just implemented the renderer.

The goal is to replicate the existing features:

* [ ] .obj file input and .bmp output.
* [ ] Several shapes (mesh, sphere, rectangle, box, etc).
* [ ] Area, ambient, and point lights.
* [ ] Photon mapping for diffuse reflection.
* [ ] Raytracing for reflective/transparent materials.
* [ ] Caustics.
* [ ] AABB raycasting optimization.
* [ ] Multisampled anti-aliasing.

With some additions:

* [ ] PNG output.
* [ ] Ability to output the different passes/layers as separate files.
* [ ] Parallelization and concurrency (use more than one core!).
* [ ] Improved multisampling.
* [ ] Improved sampling for area lights and diffuse reflections.
* [ ] Overall faster rendering speed!
* [ ] Maybe some other lighting tricks like thin films, subsurface scattering, etc.
* [ ] Tests

And some stretch goals:

* [ ] Texture mapping (and maybe normal mapping too?).
* [ ] Baked lightmap generation with three.js scene output.
* [ ] Camera modeling.
* [ ] The original code had a 3D (OpenGL) debugging mode...

The approach will be to use existing Rust crates where necessary to get things going so I don't have to rewrite *everything*, but to also build enough of it myself that I learn Rust. For example, I may decide to write my own vector libraries just for the fun of it.
