# intel-llama

Versioned Intel SYCL llama.cpp runtime used by ZimaOS Photos VLM.

- Runtime version: `2026.09.22.11060`
- llama.cpp build: `11060`
- llama.cpp revision: `4260903678a7525f43419dc234a942b551a8951e`
- Backends: SYCL and CPU
- Build profile: `photos-intel-sycl-cpu`
- Artifact: `intel-llama.raw`
- Size: `85200896` bytes
- SHA256: `410f5a8935e2b2ce4540da6bd5076203810ab8779167067a824284d1310c05fc`
- Release tag: `intel-llama-v2026.09.22.11060`

The raw filesystem is published as a GitHub Release asset rather than stored
again in Git. `intel-llama.meta.json` is the stable update index consumed by
Photos; clients use its `runtime_version` to resolve immutable release and
mirror paths.
