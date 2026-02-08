# Raycaster and Mouse Events — Three.js Journey

Project from **Three.js Journey** (Bruno Simon). Scene with 3 spheres and a duck GLB model: the Raycaster detects hover (spheres turn blue) and click, and scales up the duck on hover.

## Run

```bash
npm install
npm run dev
```

## What I learned

- **Raycaster**: cast a ray from the camera with `setFromCamera(mouse, camera)` to know which objects are under the cursor.
- **Mouse in NDC**: convert `clientX`/`clientY` to coordinates between -1 and 1 for the camera.
- **intersectObject / intersectObjects**: get the list of intersections.
- **Hover**: update the ray each frame, change color (or the duck’s scale) based on intersections.
- **Click**: use `currentIntersect` on the `click` event to identify the clicked object.
