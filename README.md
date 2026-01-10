# ordin-releases

Release feeds, installers and the memory model files for [ordin](https://github.com/gatblau/ordin).

## Memory models

The `models-1` release holds `ordin-memory-models-1.zip`, the two models ordin downloads the first time memory is used:

- `embedding/`: [`intfloat/multilingual-e5-small`](https://huggingface.co/intfloat/multilingual-e5-small), MIT licence.
- `reranker/`: [`cross-encoder/mmarco-mMiniLMv2-L12-H384-v1`](https://huggingface.co/cross-encoder/mmarco-mMiniLMv2-L12-H384-v1), Apache License 2.0.

The files are the authors' own int8 ONNX exports, unchanged. The zip carries `LICENSES.md` with both licences and a
`SHA256SUMS` for the files inside it. `SHA256SUMS` in this repository holds the zip's fingerprint; check a download with
`shasum -a 256 -c SHA256SUMS`.
