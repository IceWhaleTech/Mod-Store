# cuda-llama

Versioned CUDA llama.cpp runtime used by ZimaOS Photos VLM.

- Runtime version: `2026.08.27.10615.1`
- llama.cpp build: `10615`
- llama.cpp revision: `f280b2698`
- CUDA toolkit: `12.8.1`
- CUDA architectures: Maxwell, Pascal, Volta, Turing, Ampere, Ada, Hopper, Blackwell
- Build profile: `photos-generic-cuda`
- Artifact: `cuda-llama.raw`
- Size: `429826048` bytes
- SHA256: `12bcccf9b8b4fce05654206df395dfb30defbb7ae6da5f86e142bcb854683c16`
- Release tag: `cuda-llama-v2026.08.27.10615.1`

The runtime is not tied to RTX 3050. It ships real code for common current
architectures and PTX coverage for older or adjacent supported NVIDIA GPUs.
The Photos build keeps Q4_K, Q5_K, Q6_K, and Q8_0 MMQ kernels plus the generic
cuBLAS path used by the supported MiniCPM model and projector variants.

The large raw filesystem is published as a GitHub Release asset rather than
stored in Git. `cuda-llama.meta.json` is the stable update index consumed by
Photos; clients use its `runtime_version` to resolve the immutable release URL.
