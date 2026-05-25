# Three.js (threejs)

Three.js is an open-source JavaScript 3D library originally created by Ricardo Cabello (mrdoob) in 2010 and maintained by a broad community of contributors. It abstracts WebGL and WebGPU behind a clean object-oriented API — Scenes, Cameras, Lights, Geometries, Materials, Textures, Loaders, Controls, Animation, and Post-Processing — to make interactive 3D in the browser practical for games, product configurators, data visualization, generative art, GIS, scientific visualization, simulations, AR/VR (WebXR), and creative coding.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/threejs/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=opensource-api-evangelist&utm_content=repo)

## Tags

- 3D, Graphics, WebGL, WebGPU, JavaScript, Rendering, Open Source, Game Development, Visualization

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Project Facts

| Field | Value |
|---|---|
| Project | Three.js |
| Author | Ricardo Cabello (mrdoob) |
| First release | April 2010 |
| Current release | r184 (April 2026) |
| License | MIT |
| Package | `three` on npm (also `@types/three`) |
| Language | JavaScript / TypeScript types |
| Repository | [github.com/mrdoob/three.js](https://github.com/mrdoob/three.js) |
| Stars / forks | 113k+ / 36.4k+ |
| Renderers | WebGLRenderer (default), WebGPURenderer, SVG and CSS3D addons |
| Shading | Three.js Shading Language (TSL) — node graph compiling to GLSL and WGSL |
| Distribution | ES modules, UMD build, CDN (jsDelivr, unpkg) |

## APIs

### Three.js Core

The Three.js core library provides the scene graph, cameras, lights, geometries, materials, textures, loaders, and animation primitives used to build interactive 3D applications.

**Human URL:** [https://threejs.org/docs/](https://threejs.org/docs/)

- [Documentation](https://threejs.org/docs/)
- [Manual](https://threejs.org/manual/)
- [GitHub Repository](https://github.com/mrdoob/three.js)
- [Package — `three` on npm](https://www.npmjs.com/package/three)
- [JSON Schema — Vector3](json-schema/threejs-vector3-schema.json)
- [JSON Schema — Object3D](json-schema/threejs-object3d-schema.json)
- [JSON Schema — Scene](json-schema/threejs-scene-schema.json)
- [JSON-LD Context](json-ld/threejs-context.jsonld)

### Three.js Renderers (WebGL and WebGPU)

WebGLRenderer (default, ships in the main bundle) and WebGPURenderer (under `three/webgpu`) draw the scene graph to a canvas. The Node Material System (TSL — Three.js Shading Language) provides a unified node-based authoring model that compiles to GLSL for WebGL and WGSL for WebGPU.

- [WebGLRenderer Docs](https://threejs.org/docs/#api/en/renderers/WebGLRenderer)
- [WebGPURenderer Docs](https://threejs.org/docs/#api/en/renderers/WebGPURenderer)
- [Source — src/renderers](https://github.com/mrdoob/three.js/tree/dev/src/renderers)

### Three.js Loaders

A family of asset loaders consumed via `three/addons/loaders/*` covering glTF/GLB (recommended), OBJ, FBX, Collada, STL, PLY, 3MF, USDZ, DRACO, KTX2, Basis, and HDR/EXR environment maps.

- [Loader Documentation](https://threejs.org/docs/#api/en/loaders/Loader)
- [Source — examples/jsm/loaders](https://github.com/mrdoob/three.js/tree/dev/examples/jsm/loaders)
- [Example — glTF scene payload](examples/threejs-gltf-scene-example.json)

### Three.js Controls and Helpers

Camera and object controls shipped as addons (`three/addons/controls/*`) including OrbitControls, MapControls, TrackballControls, FirstPersonControls, FlyControls, PointerLockControls, TransformControls, DragControls, and ArcballControls.

- [OrbitControls Docs](https://threejs.org/docs/#examples/en/controls/OrbitControls)
- [Source — examples/jsm/controls](https://github.com/mrdoob/three.js/tree/dev/examples/jsm/controls)

### Three.js Post-Processing

EffectComposer plus a passes library — RenderPass, ShaderPass, UnrealBloomPass, SSAO, SSR, OutlinePass, SMAA, FXAA, TAA, Bokeh, Glitch — for chaining screen-space effects, with WebGPU equivalents under the new renderer.

- [Post-Processing Manual](https://threejs.org/docs/#manual/en/introduction/How-to-use-post-processing)
- [Source — examples/jsm/postprocessing](https://github.com/mrdoob/three.js/tree/dev/examples/jsm/postprocessing)

### Three.js Editor

Browser-based scene editor for assembling Three.js scenes, importing assets, editing materials and lights, and exporting to the documented Three.js JSON object format consumable by `ObjectLoader`.

- [Editor — threejs.org/editor](https://threejs.org/editor/)
- [Source — editor/](https://github.com/mrdoob/three.js/tree/dev/editor)

## Common Properties

- [Portal — threejs.org](https://threejs.org)
- [Documentation — threejs.org/docs](https://threejs.org/docs/)
- [Manual — threejs.org/manual](https://threejs.org/manual/)
- [Examples — threejs.org/examples](https://threejs.org/examples/)
- [Editor — threejs.org/editor](https://threejs.org/editor/)
- [GitHub Repository — mrdoob/three.js](https://github.com/mrdoob/three.js)
- [Releases / ChangeLog](https://github.com/mrdoob/three.js/releases)
- [MIT License](https://github.com/mrdoob/three.js/blob/dev/LICENSE)
- [Contributing](https://github.com/mrdoob/three.js/blob/dev/CONTRIBUTING.md)
- [Code of Conduct](https://github.com/mrdoob/three.js/blob/dev/CODE_OF_CONDUCT.md)
- [Wiki](https://github.com/mrdoob/three.js/wiki)
- [Migration Guide](https://github.com/mrdoob/three.js/wiki/Migration-Guide)
- [Discourse Forum](https://discourse.threejs.org/)
- [Discord](https://discord.gg/56GBJwAnUS)
- [Stack Overflow tag](https://stackoverflow.com/questions/tagged/three.js)
- [Package — `three` on npm](https://www.npmjs.com/package/three)
- [Package — `@types/three`](https://www.npmjs.com/package/@types/three)
- [Three.js TypeScript types](https://github.com/three-types/three-ts-types)
- [CDN — jsDelivr](https://cdn.jsdelivr.net/npm/three/)
- [CDN — unpkg](https://unpkg.com/three/)

## Integrations and Ecosystem

- [React Three Fiber](https://github.com/pmndrs/react-three-fiber)
- [drei — R3F helpers](https://github.com/pmndrs/drei)
- [A-Frame](https://github.com/aframevr/aframe)
- [`<model-viewer>`](https://github.com/google/model-viewer)
- [Threlte (Svelte)](https://github.com/threlte/threlte)
- [TroisJS (Vue)](https://github.com/troisjs/trois)
- [stats.js](https://github.com/mrdoob/stats.js)
- [Three.js DevTools](https://github.com/threejs/three-devtools)

## Artifacts

Machine-readable specifications organized by format.

### JSON Schema

- [Vector3](json-schema/threejs-vector3-schema.json)
- [Object3D](json-schema/threejs-object3d-schema.json)
- [Scene (Three.js JSON Object format)](json-schema/threejs-scene-schema.json)

### JSON-LD

- [Three.js Context](json-ld/threejs-context.jsonld)

### Examples

- [glTF scene payload](examples/threejs-gltf-scene-example.json)

### Vocabulary

- [Three.js Vocabulary](vocabulary/threejs-vocabulary.yml)

## Notes

Three.js is a pure client-side / runtime JavaScript library. It does not expose a hosted REST or AsyncAPI surface and therefore this profile intentionally omits OpenAPI / AsyncAPI / Naftiko capability artifacts. The machine-readable contracts that matter for Three.js are its JSON scene format (covered here as JSON Schema and JSON-LD) and the broader asset loader formats (glTF, USDZ, FBX) it supports as inputs.

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
