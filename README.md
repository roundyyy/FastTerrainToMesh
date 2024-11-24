# Fast Terrain To Mesh Converter Generator for Unity Mobile and VR

A Unity tool for efficient terrain-to-mesh conversion with a highly optimized unlit shader, perfect for VR, mobile, and performance-critical applications.

![Terrain To Mesh Screenshot](screenshot.png)

[![Demo Scene Made With This Tool](http://img.youtube.com/vi/Sw4tQi6weog/0.jpg)](http://www.youtube.com/watch?v=Sw4tQi6weog "Demo Scene Made With This Tool")

*The scene in this demo was created using this terrain conversion tool.*

## Features

- **Fast Terrain Conversion**:
  - Convert Unity terrains to mesh chunks with texture splatmaps.
  - Optional generation of LOD levels for terrain chunks for efficient rendering.
    - **Warning**: Gaps between LOD levels may occur. Use more advanced mesh simplifiers for seamless transitions.
- **Highly Optimized Shader**:
  - Unlit shader compatible with Built-in Render Pipeline (BIRP) and Universal Render Pipeline (URP).
  - Minimal GPU usage, ideal for VR and mobile applications.
  - Supports up to 4 terrain textures using Texture Arrays.
  - Optional lightmap and smoothness effects.
  - Distance-based texture resampling to prevent tiling artifacts.
  - Height-based texture blending and customizable texture tiling.
- **Customizable Output**:
  - Adjustable chunk size and resolution.
  - Control over mesh colliders and static flags.
  - Options for handling the original terrain (disable, hide, or keep enabled).
  - Built-in terrain tree exporter to convert terrain trees into scene objects.
  - Flexible splat and texture array resolution settings.

## Installation

1. Download the latest release package from the [Releases](https://github.com/yourusername/FastTerrainToMeshGenerator/releases) page.
2. Import the package into your Unity project.
3. The tool will be available under `Tools/Roundy/Fast Terrain To Mesh Generator`.

## Usage

1. Open the tool from Unity's menu: `Tools/Roundy/Fast Terrain To Mesh Generator`.
2. Drag your terrain into the "Source Terrain" slot.
3. Configure conversion settings:
   - **Quality Settings**: Choose between Basic and Resampling shader variants.
   - **Mesh Generation**: Adjust chunk amount, resolution per chunk, and enable LOD groups if needed.
   - **Texture Settings**: Configure splat resolution and texture array resolutions.
   - **Tree Settings**: Convert terrain trees to scene objects with customizable settings.
4. Click "Convert Terrain" to generate the mesh with the optimized shader.

## Optimization Tips

- For VR applications, use low chunk resolutions and the Basic shader quality when resampling isn't necessary.
- Enable LOD groups for better performance on large terrains.
- When generating LODs, ensure the highest resolution level matches your terrain's original quality.

## Technical Details

### Shader Features
- Unlit, vertex/fragment shader with minimal overhead.
- Supports Texture Arrays for efficient texture handling.
- Optional smoothness effect via alpha channel.
- Distance-based texture resampling to reduce noticeable tiling of textures at greater distances.
- Lightmap support for baked lighting.
- Height-based texture blending.
- Configurable tiling and offsets for up to 4 texture layers.

### Mesh Generation
- Chunk-based mesh generation for optimized memory usage.
- Optional LOD levels with customizable reduction strength and transition heights.
- Supports mesh colliders and static object flags.
- Terrain tree exporter with LOD and parent group handling.
- Accurate heightmap sampling for precise terrain recreation.

## Future Updates

- **Lit Shader Version**: Including normal map support for enhanced visual fidelity.
- **Improved LOD Transitions**: Seamless transitions between LOD levels.
- Additional optimization settings and shader features.

## Requirements

- Unity 2019.4 or higher (tested up to Unity 2026).
- Supports Built-in Render Pipeline and Universal Render Pipeline.
- Designed for VR and mobile applications.

## Usage Rights

This tool is free to use for any purpose, including commercial projects.

## Support

For issues, feature requests, or questions, please use the [GitHub Issues](https://github.com/roundyy/FastTerrainToMesh/issues) page.
