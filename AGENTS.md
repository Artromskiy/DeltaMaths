# DeltaMaths agent router

Scope: portable engine-independent runtime maths and its generated CPU/shader
symbol and layout contract. Generated files are never edited directly.
Preserve netstandard2.0/2.1, std430 compatibility and the shared
column-vector CPU/GLSL convention.

## Map — open only as needed

- ../CODE_STYLE.md — technical numeric hot-path, storage, type and evidence rules.
- ../CONTRACTS.md — deterministic generation/ABI ownership; open only for a boundary task.
- IDEAS.md — research/options only when explicitly requested.
- WORKFLOW.md — generation, target builds and tests.
- docs/CPU_GPU_CONFORMANCE.md — CPU/shader/Vulkan differential-conformance protocol.
- docs/README.md — nested leaf documentation; open only for a named docs task.
- src/DeltaMaths — production runtime and generated API.
- tests, benchmarks, probes — verification, measured workloads and focused checks.
- ../DeltaMathsGen/AGENTS.md — required when generator output changes.
- ../DeltaShader/AGENTS.md — required when shader-visible identity/layout changes.

Use vectorization or simd-intrinsics for measured numeric paths,
abi-and-calling-conventions for layouts, shader-dev for mappings, and
performance-benchmark only for an explicit bounded comparison.
