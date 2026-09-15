# 3D File Viewer

An interactive WebGL-based 3D model viewer for exploring 3D geometry files.

## Features

- **Interactive 3D Visualization** - Smooth orbit, pan, and zoom controls
- **Wireframe Mode** - Toggle between shaded and wireframe rendering
- **Grid & Axes** - Visualize coordinate system and ground plane
- **Parts Management** - Show/hide individual parts with visibility controls
- **Color Customization** - Override part colors with custom color picker
- **Auto-rotate** - Automatic rotation with adjustable speed
- **Dark Mode** - Switch between light and dark themes
- **Part Isolation** - Double-click to focus on individual parts
- **Screenshot Export** - Save PNG snapshots of your 3D model
- **Touch Support** - Full multi-touch gesture support (pinch-to-zoom)
- **Responsive Design** - Works on desktop and mobile devices

## Usage

### View the 3D Model

**[🚀 View the 3D Viewer](https://adrian-locke.github.io/3D_FILE_VIEWER/)**

Or access the viewer directly with your own model files:
```
viewer.html?model=your_file.json
```

## Controls

| Action | Control |
|--------|---------|
| Orbit | Drag with left mouse button |
| Pan | Right-click drag or Shift + drag |
| Zoom | Scroll wheel or pinch (mobile) |
| Select Part | Click on model |
| Isolate Part | Double-click on model |
| Fit View | Press `F` or click Fit View |
| Toggle Wireframe | Press `W` or click Wireframe |
| Toggle Grid | Press `G` or click Grid |
| Toggle Axes | Press `A` or click Axes |
| Save PNG | Press `S` or click Save PNG |
| Show Parts | Press `P` or click Parts |

## File Format

Models must be in JSON format with the following structure:

```json
{
  "bounds": {
    "min": [-x, -y, -z],
    "max": [x, y, z]
  },
  "center": [x, y, z],
  "parts": ["Part Name 1", "Part Name 2"],
  "colors": [[r, g, b], [r, g, b]],
  "chunks": [
    {
      "part": 0,
      "pos": [x1, y1, z1, x2, y2, z2, ...],
      "nrm": [nx1, ny1, nz1, nx2, ny2, nz2, ...],
      "idx": [i1, i2, i3, ...]
    }
  ]
}
```

## Technologies

- **WebGL** - Hardware-accelerated 3D rendering
- **HTML5** - Modern web standards
- **Canvas API** - Drawing and rendering
- **Vanilla JavaScript** - No external dependencies

## Author

Created by [adrian-locke](https://github.com/adrian-locke)

---

**Enjoy exploring your 3D models!** 🎨✨