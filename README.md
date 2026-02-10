# VRPM-Roofy

A web-based 3D measurement tool for roof modeling and surface area calculation. Built with Three.js, this single-file application allows you to upload 3D models, measure areas, and calculate tile counts.

## Features

### 🎯 Core Functionality
- **Multi-format support**: OBJ, FBX, GLB/GLTF with texture loading
- **Three measurement modes**:
  - **Orbit**: Navigate and inspect your model
  - **Measure**: Draw polygons on surfaces to calculate area
  - **Tape**: Measure distances between two points
- **Real-time calculations**: Area in m², tile count with wastage

### 🎨 Visualization
- **Three shading modes**:
  - Original (textured/unlit)
  - Clay (uniform grey with depth)
  - Normals (color-coded by surface orientation)
- **Model rotation controls** for Z-up/Y-up conversion
- **Floating 3D labels** for tape measurements

### 📐 Measurements
- **Polygon area tool**: Click points on the model surface to create measurement polygons
- **Tape measure**: Two-point distance measurement with floating labels
- **Unit support**: mm, cm, m, or custom units
- **Tile calculator**: Automatic tile count with configurable wastage %

## Usage

1. **Open `index.html`** in a modern web browser (Chrome, Firefox, Edge)
2. **Load a model**: Drag and drop your 3D model file (+ textures if applicable)
3. **Set units**: Choose the unit scale of your model (mm/cm/m)
4. **Measure**:
   - Switch to **Measure mode** to draw area polygons
   - Switch to **Tape mode** to measure distances
   - Use **Orbit mode** to navigate
5. **Calculate tiles**: Enter tile dimensions and wastage percentage

## Technical Details

- **Built with**: Three.js r169 (loaded from CDN)
- **Architecture**: Single self-contained HTML file
- **No build step**: Open directly in browser
- **File size**: ~50KB (uncompressed)

## Keyboard Shortcuts

- `M` - Toggle Measure mode
- `Enter` - Close polygon (in Measure mode)
- `Backspace` - Undo last point
- `Esc` - Return to Orbit mode

## Model Requirements

- Supported formats: `.obj`, `.fbx`, `.glb`, `.gltf`
- Textures: Drop `.jpg`/`.png` files alongside the model
- OBJ materials: Drop `.mtl` file with the model

## Browser Compatibility

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## License

This project is provided as-is for educational and commercial use.

---

**Co-Authored-By**: Claude Sonnet 4.5
