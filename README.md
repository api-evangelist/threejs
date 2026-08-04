# Three.js (threejs)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
