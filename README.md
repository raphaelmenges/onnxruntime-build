# ONNX Runtime Build

Fork of <https://github.com/supertone-inc/onnxruntime-build>.

## How to release a new version

1. Upgrade the submodule `onnxruntime` with the new version of the ONNX runtime. You can check the releases or tags [in their repository](https://github.com/microsoft/onnxruntime).
1. Upgrade the ONNX runtime version in `ONNXRUNTIME_VERSION` accordingly.
1. Create a new tag of the version in the repository via `git tag vX.X.X` and push it to GitHub via `git push origin --tags`.
1. The `Build` workflow of GitHub actions should be automatically triggered by the new tag and after a few minutes a new release should be listed in this GitHub repository.