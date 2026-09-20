# cpu-llama

Versioned x86_64 AVX2 CPU llama runtime used by ZimaOS Photos VLM.

- Runtime version: `2026.09.04.1`
- llama.cpp revision: `7c203670f8d746382247ed369fea7fbf10df8ae0`
- Backend: CPU
- Build profile: `photos-generic-cpu`
- Artifact: `cpu-llama.raw`
- Size: `4120576` bytes
- SHA256: `6a8d1e7672bf70938da771d02d4b1e16aff642e5b6aa94f8db4cb80b43359a88`
- Release tag: `cpu-llama-v2026.09.04.1`

The raw filesystem is published as a GitHub Release asset rather than stored
in Git. `cpu-llama.meta.json` is the stable update index consumed by Photos;
clients use its `runtime_version` to resolve immutable release and mirror paths.
