FastNoiseLite port for Godot Engine shaders
============================================

This is a port of [FastNoiseLite](https://github.com/Auburn/FastNoiseLite) to Godot shaders. It is handy if you are interested in having the same results between the CPU-based version and shaders.

The code has room for improvement. It was ported roughly from the HLSL version, with no particular GPU optimizations. If you are looking for the fastest GPU noise around, I would recommend a tailored version instead of this one.

Godot doesn't support `#include` and does not support "includable shader" libraries, so the library is currently in a CanvasItem shader alongside some testing code. If you want to use it, you have to copy the library code in your shaders.
