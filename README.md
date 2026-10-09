# salt-llvm-patches
Minimal repository to be used as a submodule containing llvm [CMake] patches
for [SALT-FM].
These patches must be applied to the installed LLVM [Cmake] files
_unless a full installation of LLVM and Clang is present_.
If a full installation of LLVM and/or Clang is not present,
configuring [SALT-FM] with [CMake] will throw an error because there are
missing LLVM/Clang components.

This repository is intended to be used as a git submodule to share the
definition of the patches to the installed LLVM [Cmake] files required by
the [SALT-FM] project.
The containerized [SALT-FM development environment] needs to apply these
patches as well, however their definitions are more tightly tied to
the [SALT-FM] project itself.

[SALT-FM]: https://github.com/ParaToolsInc/SALT-FM
[SALT-FM development environment]: https://github.com/ParaToolsInc/salt-dev
[CMake]: https://cmake.org/
