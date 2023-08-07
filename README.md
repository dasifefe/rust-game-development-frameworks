<h1 align="center">Libraries and frameworks for <br>Game Development in Rust</h1>

<p align="center">
  <img src="./community-icon.png">
</p>

<h2 align="center">Join the <a href="https://discord.gg/yNtPTb2"><u>Game Development in Rust</u></a> Discord server</h2>

This curated list is from the **Game Development in Rust** Discord server and prioritizes libraries and frameworks that have examples and are ready or almost ready for production.

For a longer list of libraries and frameworks, see [Are We Game Yet?](https://arewegameyet.rs).

## Rust basics

- [Rust book](https://doc.rust-lang.org/book/).
- [Standard library - Comprehensive guide to the Rust standard library APIs](https://doc.rust-lang.org/std/index.html).
- [Edition guide - Guide to the Rust editions](https://doc.rust-lang.org/edition-guide/index.html).
- [Cargo book - A book on Rust’s package manager and build system](https://doc.rust-lang.org/cargo/index.html).
- [Rustdoc book - Learn how to make awesome documentation for your crate](https://doc.rust-lang.org/rustdoc/index.html).
- [Rustc book - Familiarize yourself with the knobs available in the Rust compiler](https://doc.rust-lang.org/rustc/index.html).
- [Compiler error index - In-depth explanations of the errors you may see from the Rust compiler](https://doc.rust-lang.org/error-index.html).

## Resources to understand ECS (Entity Component System) and DOD (Data-Oriented Design)

ECS/DOD is quite a big deal in Rust. Here are some resources to understand the basics:

- [Understanding data-oriented design for entity component systems - Unity at GDC 2019](https://www.youtube.com/watch?v=0_Byw9UMn9g).
- [CppCon 2018: Stoyan Nikolov “OOP Is Dead, Long Live Data-oriented Design”](https://www.youtube.com/watch?v=yy8jQgmhbAU) - Harsh title (ECS/DOD is not a silver bullet for every problem), but useful regardless.
- [RustConf 2018 - Closing Keynote - Using Rust For Game Development by Catherine West](https://www.youtube.com/watch?v=aKLntZcp27M) - A classic presentation already - Catherine West gives several examples, explain the problems with them, and shows the alternatives.
- ["Data-Oriented Design" web book by Richard Fabian](https://dataorienteddesign.com/dodbook).

## Productivity tools for game development

- [Blender](https://www.blender.org) for 3D modeling.
- [Krita](https://krita.org/en) for 2D image creation.

## Game engines

### 2D + 3D

Recommended if you are going to work with 3D graphics, however, API changes still might happen in future releases.

- [bevy](https://bevyengine.org) Refreshingly simple data-driven game engine.
- [ambient](https://docs.rs/ambient_api) Runtime for building high-performance multiplayer games and 3D applications, powered by WebAssembly, Rust and WebGPU.
- [fyrox](https://docs.rs/fyrox) Feature-rich, production-ready, general purpose 2D/3D game engine written in Rust with a scene editor. Formerly known as `rg3d`.
- [hotham](https://docs.rs/hotham) lightweight, high performance game engine for standalone VR headsets.

### 2D

Recommended if you are going to work strictly with 2D graphics.

- [emerald](https://docs.rs/emerald)
- [macroquad](https://docs.rs/macroquad)
- [ggez](https://docs.rs/ggez)
- [tetra](https://docs.rs/tetra)
- [oxygengine](https://docs.rs/oxygengine)

## Open-Source Games

Some open-source games made in Rust:

- [RecWars](https://github.com/martin-t/rec-wars) A multiplayer top-down tank shooter. Already has some basic gameplay and a playable browser version.
- [RustCycles](https://github.com/rustcycles/rustcycles) A third person arena shooter that's about movement, not aim. You have to be smart and think fast.
  - State of development: *This is just barely a prototype. There's no real gameplay yet, just the engine's default physics and some primitive networking.*

## Graphics-only

- [wgpu](https://docs.rs/wgpu) Cross-platform, safe, pure-rust graphics api (Vulkan, Metal, D3D12, D3D11, OpenGLES, WebGPU).
  - [WebGPU specification here](https://www.w3.org/TR/webgpu).
  - [Learn WGPU - tutorial](https://sotrh.github.io/learn-wgpu).
  - [Learn WGPU - tutorial in video](https://www.youtube.com/playlist?list=PLWtPciJ1UMuBs_3G-jFrMJnM5ZMKgl37H).
- [rend3](https://docs.rs/rend3) Easy to use, customizable, efficient 3D renderer library. Built on top of `wgpu`.
- [rafx](https://docs.rs/rafx) Multi-backend renderer that prioritizes performance, flexibility, and productivity.
- [ash](https://docs.rs/ash) Low-level bindings to Vulkan.
- [lyon](https://docs.rs/lyon) GPU-based 2D vector rendering. Built on top of `wgpu`.
- [luminance](https://docs.rs/luminance) High level. Built on top of OpenGL.
- [miniquad](https://docs.rs/miniquad) High-level. Focus on portability. Built on top of OpenGL, GLES 3 and WebGl1.
- [golem](https://docs.rs/golem) Intermediate-level. Higher level wrapper built on glow.
- [vulkano](https://docs.rs/vulkano) Intermediate-level. Safer wrapper for Vulkan.
- [glow](https://docs.rs/glow) Low-level. Safer wrapper for OpenGL and WebGL.
- [erupt](https://docs.rs/erupt) Low-level bindings to Vulkan.
- [gl46](https://docs.rs/gl46) Low-level. Wrapper for OpenGL 4.6 (generated by Phosphorus).
- [gl33](https://docs.rs/gl33) Low-level. Wrapper for OpenGL 3.3 (generated by Phosphorus).
- [screen-13](https://docs.rs/screen-13) Screen 13 is an easy-to-use Vulkan rendering engine in the spirit of QBasic.
- [sierra](https://docs.rs/sierra) Low-level control and high-level features. Built on top of `erupt`.

I believe it is fair to say that if you use libraries built on top of WGPU, you will get wider support on modern platforms (Linux, Windows, MacOS, Android and iOS).

## Window creation and OS integration

- [winit](https://docs.rs/winit) Rusty windowing framework. The *de facto* standard in the Rust community.
- [glfw](https://docs.rs/glfw) Rust wrapper for the C GLFW3 library.
- [fermium](https://docs.rs/fermium) Rust wrapper for the C SDL2 library. Contains more than window creation features.
- [sdl2](https://docs.rs/sdl2) Rust wrapper for the C SDL2 library. Contains more than window creation features.

## Frameworks for ECS

- [hecs](https://docs.rs/hecs) Archetype-based.
- [yaks](https://docs.rs/yaks) Add multi-threading to `hecs`.
- [legion](https://docs.rs/legion) Archetype-based.
- [shipyard](https://docs.rs/shipyard) Sparse-based.
- [specs](https://docs.rs/specs) Bitset-based.

See [this repository](https://github.com/SanderMertens/ecs-faq#what-are-the-different-ways-to-implement-an-ecs) for information on the different types of ECS (archetype, sparse, bitset).

## Frameworks for physics and linear math (for 2D and 3D programming)

- [glam](https://docs.rs/glam)
- [rapier2d](https://docs.rs/rapier2d) / [rapier3d](https://docs.rs/rapier3d) New 2D/3D physics framework from the creator of `nphysics2D`/`nphysics3D`. [2D demo](https://rapier.rs/demos2d/index.html) and [3D demo](https://rapier.rs/demos3d/index.html).
- [cgmath](https://docs.rs/cgmath)
- [nalgebra](https://docs.rs/nalgebra)
- [ultraviolet](https://docs.rs/ultraviolet)
- [vek](https://docs.rs/vek)

## Graphical user interface (GUI)

- [yakui](https://github.com/LPGhatguy/yakui) Combines a layout model inspired by Flutter with the ease-of-use of an immediate mode UI library like Dear Imgui or egui.
- [egui](https://docs.rs/egui/) Pure Rust cross-platform library. Many renderers already have an integration with `Egui`.
- [iced](https://docs.rs/iced/) Pure Rust cross-platform library.
- [imgui](https://docs.rs/imgui/) Bindings in Rust for the Dear ImGui C++ library.

## Font (parser and/or rasterizer)

- [fontdue](https://docs.rs/fontdue)
- [swash](https://github.com/dfrg/swash)
- [rustybuzz](https://docs.rs/rustybuzz) Complete harfbuzz shaping algorithm port to Rust.
- [ttf-parser](https://docs.rs/ttf-parser) High-level, safe, zero-allocation TrueType font parser.

## Space partitioning 

- [rstar](https://docs.rs/crate/rstar/) N-dimensional [r*-tree](https://en.wikipedia.org/wiki/R*_tree) implementation
- [bvh](https://docs.rs/crate/bvh/) Bounding Volume Hierarchy, built on top of [nalgebra](https://www.nalgebra.org/).
- [kdtree](https://docs.rs/crate/kdtree/) K-dimensional tree in Rust for fast geospatial indexing and nearest neighbors lookup.
- [ncollide 2D](https://docs.rs/crate/ncollide2d/) Bounding Volume Tree implementation [(2d documentation)](https://www.ncollide.org/rustdoc/ncollide2d/partitioning/struct.BVT.html).
- [ncollide 3D](https://docs.rs/crate/ncollide3d/) Bounding Volume Tree implementation [(3d documentation)](https://www.ncollide.org/rustdoc/ncollide3d/partitioning/struct.BVT.html).
- [spade](https://docs.rs/crate/spade/) Implements  [r*-tree](https://en.wikipedia.org/wiki/R*_tree) and [delaunay triangulation](https://en.wikipedia.org/wiki/Delaunay_triangulation).
- [flat_spatial](https://docs.rs/crate/flat_spatial/) Simple flat structures such as a grid/hashmap of cells.
- [acacia](https://docs.rs/crate/acacia/)  Generic over the dimension of the partitioned space and thus supports binary trees, quadtrees, octrees, etc.

## Network

- [tokio](https://docs.rs/tokio) Asynchronous TCP and UDP sockets.
- [quinn](https://docs.rs/quinn) QUIC transport protocol implementation. Built on top of `tokio`.

## Audio

- [oddio](https://docs.rs/oddio) Built on top of `cpal`.
- [kira](https://docs.rs/kira) Built on top of `cpal`.
- [rodio](https://docs.rs/rodio) Built on top of `cpal`.
- [cpal](https://docs.rs/cpal) Low-level cross-platform library for audio input and output.
- [alto](https://docs.rs/alto) Wrapper for OpenAL.
- [openal](https://docs.rs/openal) Wrapper for OpenAL.

## Serialization-Deserialization

- [redb](https://docs.rs/redb) Embedded key-value database in pure Rust.
- [speedy](https://docs.rs/speedy) Fast, simple and easy binary serialization.
- [serde](https://docs.rs/serde) Serialize and deserialize data structures efficiently and generically.
- [serde-json](https://crates.io/crates/serde_json) Serialize and deserialize for **JSON format**. Built on top of `serde`.
- [bincode](https://crates.io/crates/bincode) Serialize and deserialize for **binary format**. Built on top of `serde`.
- [borsh](https://docs.rs/borsh) Implementation of the Borsh (Binary Object Representation Serializer for Hashing) binary serialization format. It is meant to be used in security-critical projects as it prioritizes consistency, safety, speed, and comes with a strict specification.

## Other utilities

- [thunderdome](https://docs.rs/thunderdome) ~~Gladitorial~~ generational arena inspired by generational-arena, slotmap, and slab. It provides constant time insertion, lookup, and removal via small keys returned from `Arena`.
- [hexasphere](https://docs.rs/hexasphere) Subdivide 3D shapes (icosahedron, tetrahedron, square, triangle, cube) made of triangles.
- [navmesh](https://docs.rs/navmesh/) Navigation mesh path-finder.
- [density-mesh-core](https://docs.rs/density-mesh-core) / [density-mesh-image](https://docs.rs/density-mesh-image) Generate 2D mesh from images representing density/height map.
- [image](https://docs.rs/image) Image encoding and decoding for many image formats.
- [rayon](https://docs.rs/rayon) Introduce parallelism into existing code and guarantees data-race free executions.
- [palette](https://docs.rs/palette) Linear color calculations.
- [pathfinding](https://docs.rs/pathfinding) Multiple implementations of path-finding algorithms.
- [salva2d](https://docs.rs/salva2d) / [salva3d](https://docs.rs/salva3d) Particle-based fluid dynamics.
- [collider](https://docs.rs/collider) Continuous 2D collision detection.
