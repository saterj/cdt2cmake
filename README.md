# cdt2cmake

[![Actions Status](https://badgen.net/github/checks/saterj/cdt2cmake?icon=github&label=Build%20Status)](https://github.com/saterj/cdt2cmake/actions)

> Eclipse CDT to CMake converter

An ugly, awful, hackish utility written to liberate code from Eclipse CDT.

Works only for Managed Builder CDT projects on linux. Probably doesn't work for complicated (= build configuration per folder) managed build projects.

Works good enough for my purposes, ~not likely to~ _definately won't_ be improved. But it will be altered.

The eclipse CDT model does not map directly to the CMake model so files generated by this tool will almost certainly need touching up.

## build 
`cmake --build .`

## Usage
```bash
cdt2make [--generate] proj1 [...projn]
```

The `--generate` flag will write the `CMakeLists.txt` files to their respective subfolders. Default without generate is to write the contents of the CMakeLists.txt files to stdout.

