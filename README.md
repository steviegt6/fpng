# libfpng

**libfpng** is a fork of [richgel999/fpng](https://github.com/richgel999/fpng) that switches from a single-file header to a DLL. It's designed specifically for [steviegt6/fnb](https://github.com/steviegt6/libfpng).

This fork does away with the single-file header, dependency-less approach:

- it leverages [libdeflate](https://github.com/ebiggers/libdeflate)'s CRC32 and Adler32 implementations.
