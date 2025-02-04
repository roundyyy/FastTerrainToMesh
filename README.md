# Fast Terrain To Mesh Converter Generator for Unity Mobile and VR

A Unity tool for efficient terrain-to-mesh conversion with optimized shaders, perfect for VR, mobile, and performance-critical applications.

![Terrain To Mesh Screenshot](screenshot.png)

## Demo

[<img src="https://img.youtube.com/vi/Sw4tQi6weog/maxresdefault.jpg" width="600px" alt="Click to Watch Demo Video">](https://youtu.be/Sw4tQi6weog)
#### 🎥 Click image to watch demo video

*The scene in this demo was created using this terrain conversion tool.*

## Features

### Terrain Conversion
- Convert Unity terrains to optimized mesh chunks with texture splatmaps
- LOD level generation with customizable transition heights and reduction strength
- Configurable chunk size and resolution
- Mesh collider and static flag options
- Flexible terrain handling (disable, hide, or keep enabled)

### Shader Options
- Multiple shader variants:
  - Unlit shader for maximum performance
  - Lit shader for Built-in Render Pipeline (BIRP)
  - Lit shader for Universal Render Pipeline (URP)
- Normal map support for enhanced visual detail
- Support for up to 4 terrain textures using Texture Arrays
- Optional lightmap and smoothness effects
- Distance-based texture resampling
- Height-based texture blending
- Customizable texture tiling

### Vegetation Export
- Tree conversion with full hierarchy preservation
- Detail object export supporting both:
  - Texture-based grass/details
  - Prefab-based vegetation
- Density control and placement optimization
- LOD support for tree prefabs
- Customizable detail spawn settings

### Mesh Adjustment Tool
- Fix floating or sunken objects after terrain conversion
- Bulk adjustment of vegetation and props to terrain height
- Surface normal alignment options
- Configurable sink depth
- Debug visualization mode
- Fast processing mode for large object sets

## Installation

1. Download the latest release package from the [Releases](https://github.com/roundyyy/FastTerrainToMesh/releases) page.
2. Import the package into your Unity project.
3. The tool will be available under `Tools/Roundy/Fast Terrain To Mesh Generator`.

## Requirements

- Unity 2019.4 or higher (tested up to Unity 6)
- Supports Built-in Render Pipeline and Universal Render Pipeline
- Designed for VR and mobile applications

## Support

For issues, feature requests, or questions, please use the [GitHub Issues](https://github.com/roundyy/FastTerrainToMesh/issues) page.

## Usage Rights

This tool is free to use for any purpose, including commercial projects.
