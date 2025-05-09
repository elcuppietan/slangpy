.. _changelog:

.. cpp:namespace:: sgl

Changelog
=========

SlangPy uses a `semantic versioning <http://semver.org>`__ policy for its API.

Version 0.27.0 (TBA)
----------------------------

- Introduce basic support for bindless textures and samplers. Currently only supported on D3D12.
  Add ``sgl::Feature::bindless`` (``slangpy.Feature.bindless``) to detect bindless support.
  Add ``sgl::DescriptorHandle`` (``slangpy.DescriptorHandle``) to represent bindless descriptor handles.
  Add ``sgl::Sampler::descriptor_handle()`` (``slangpy.Sampler.descriptor_handle``) to get the descriptor handle for a sampler.
  Add ``sgl::Texture::descriptor_handle_ro()`` (``slangpy.Texture.descriptor_handle_ro``) to get the read-only descriptor handle for a texture.
  Add ``sgl::Texture::descriptor_handle_rw()`` (``slangpy.Texture.descriptor_handle_rw``) to get the read-write descriptor handle for a texture.
  (PR `#196 <https://github.com/shader-slang/slangpy/pull/196>`__).
- Rename ``sgl::Struct`` to ``sgl::DataStruct`` to match ``slangpy.DataStruct``.
  Rename ``sgl::StructConverter`` to ``sgl::DataStructConverter``
  and ``slangpy.StructConverter`` to ``slangpy.DataStructConverter``.
  (PR `#185 <https://github.com/shader-slang/slangpy/pull/185>`__).


Version 0.26.0
----------------------------

- Port samples to use new combined SlangPy/SGL API
- CUDA and Metal fixes
- Initial deployment of wheels for macOS


Version 0.25.0
----------------------------

- Fix deploying slangpy shader files


Version 0.24.0
----------------------------

- Merge SGL (https://github.com/shader-slang/sgl) into SlangPy.

Version 0.23.0
----------------------------

- Require SGL v0.15.0
- Refactor of NDBuffer and Tensor to share some underlying type
- NDBuffer and Tensor support indexing

Version 0.22.0
----------------------------

- Requre new SGL v0.14.0 with switch to Slang-RHI

Version 0.21.1
----------------------------

- Fix to numpy version requirement
- Fixes to examples
- Add neural network example
- Require SGL v0.13.1

Version 0.21.0
----------------------------

- Full Jupyter notebook support
- Lots of fixes for edge-case hot reload crashes
- Significantly more robust wang hash and rand float generators
- Direct return of structs from scalar calls
- Add diff splatting sample
- Fix for rare issue involving lookup order of generic functions vs generic types
- Require SGL v0.13.0

Version 0.20.1
----------------------------

- Fix scalar wang-hash arg types

Version 0.20.0
----------------------------

- Add SDF example
- Transpose vector coordinates

Version 0.19.5
----------------------------

- Documentation for generators
- Extra fixes for grid

Version 0.19.4
----------------------------

- Fix grid issue

Version 0.19.3
----------------------------

- Update SGL -> 0.12.4
- Significant improvements to generator types
- Support textures as output type

Version 0.19.2
----------------------------

- Update SGL -> 0.12.3
- Better error messages during generation
- Fix corrupt error tables
- Restore detailed error information during dispatch

Version 0.19.1
----------------------------

- Update SGL -> 0.12.2
- Fix major issue with texture transposes

Version 0.19.0
----------------------------

- Add experimental grid type

Version 0.18.2
----------------------------

- Update SGL -> 0.12.1
- Rename from_numpy to buffer_from_numpy

Version 0.18.1
----------------------------

- Fix Python 3.9 typing

Version 0.18.0
----------------------------

- Long file temp filenames fix
- Temp fix for resolution of types that involve generics in multiple files
- Support passing 1D NDBuffer to structured buffer
- Fix native buffer not being passed to bindings
- Missing slang field check
- Avoid synthesizing store methods for none-written nested types

Version 0.17.0
----------------------------

- Update to latest `nv-sgl` with CoopVec support
- Native tensor implementation
- Linux crash fix

Version 0.16.0
----------------------------

- Native texture and structured buffer implementations
- Native function dispatches
- Lots of bug fixes

Version 0.15.2
----------------------------

- Correctly package slang files in wheel

Version 0.15.0
----------------------------

- Native buffer takes full reflection layout
- Add uniforms + cursor api to native buffer
- Update required version of `nv-sgl` to `0.9.0`

Version 0.14.0
----------------------------

- Update required version of `nv-sgl` to `0.8.0`
- Substantial native + python optimizations

Version 0.13.0
----------------------------

- Update required version of `nv-sgl` to `0.7.0`
- Native SlangPy backend re-enabled
- Conversion of NDBuffer to native code
- PyTorch integration refactor

Version 0.12.0
----------------------------

- Update required version of `nv-sgl` to `0.6.2`
- Re-enable broken Vulkan tests

Version 0.12.0
----------------------------

- Update required version of `nv-sgl` to `0.6.1`

Version 0.10.0
----------------------------

- Initial test release
