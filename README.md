Simple, self-contained WebGL solar system animation built with Three.js. It uses free, high-quality planet textures from Solar System Scope (based on NASA data, CC BY 4.0) and requires no build tools—just save the code as an HTML file and open it in a browser.

### Free textures used

All planet textures come from **Solar System Scope** (`solarsystemscope.com/textures`). They are based on NASA elevation and imagery data and are released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license, so you can use, adapt, and share them for any purpose—even commercially. The exact files loaded in the code are:

- Sun: `2k_sun.jpg`
- Mercury: `2k_mercury.jpg`
- Venus: `2k_venus_surface.jpg`
- Earth: `2k_earth_daymap.jpg`
- Mars: `2k_mars.jpg`
- Jupiter: `2k_jupiter.jpg`
- Saturn: `2k_saturn.jpg`
- Uranus: `2k_uranus.jpg`
- Neptune: `2k_neptune.jpg`
- Starfield: `2k_stars_milky_way.jpg`

### How it works (quick overview)

1. **Scene & camera** – A perspective camera and `OrbitControls` let you drag and zoom.
2. **Lighting** – A point light at the Sun's centre illuminates the planets; ambient light prevents pitch-black night sides.
3. **Starfield** – A large inverted sphere is textured with a Milky Way map.
4. **Sun** – A basic material with an emissive texture, plus a faint translucent “glow” sphere.
5. **Planets** – Each is a `SphereGeometry` with a `MeshStandardMaterial` and its own texture. They orbit at different speeds and spin on their axes.
6. **Saturn’s ring** – A simple transparent ring mesh is attached as a child of Saturn (you can delete that block if you want it even simpler).
7. **Animation** – `requestAnimationFrame` updates orbital angles and rotation each frame, while `OrbitControls` handles camera damping.

### Disclaimer
This is a **quick test project**, built in a single sitting as a way to
experiment with WebGL and Three.js. It was generated with the help of
an AI assistant (DeepSeek) and is **not** production-ready code.

Feel free to fork, remix, or use it as a starting point for your own
experiments.
