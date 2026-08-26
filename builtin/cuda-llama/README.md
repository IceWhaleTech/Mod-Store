# cuda-llama

Versioned CUDA llama.cpp runtime used by ZimaOS Photos VLM.

- Runtime version: `2026.08.26.10615`
- llama.cpp build: `10615`
- llama.cpp revision: `f280b2698`
- Artifact: `cuda-llama.raw`
- Size: `766066688` bytes
- SHA256: `30b05111518c62a2c32ea5d10299aaca8475245fd6f98a086e9f4b8963a6eb8f`
- Release tag: `cuda-llama-v2026.08.26.10615`

The large raw filesystem is published as a GitHub Release asset rather than
stored in Git. `cuda-llama.meta.json` is the stable update index consumed by
Photos; clients use its `runtime_version` to resolve the immutable release URL.
