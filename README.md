# What is it
Xcode project to build an custom toolchain for Xcode based on llvm/clang. 

# Features
- [x] makefile based project to build own custom toolchain for macOS
- [x] one makefile to define used versions (Makefile.def)
- [x] download required source (i.e. cmake, llvm ...)

# Usage
0. Adapt PROXY_SETTINGS_HTTP (Makefile.dlf) if you want to use proxy settings.
1. Select scheme `download` and build to download required source.
2. Select scheme `build-toolchain` and build to build custom toolchain, as result you get an *tar.gz package.
3. Select scheme `install-toolchain` and build to install toolchain for local user.

# Tests
- Tested with macOS 10.11 and Xcode 8.2.1
