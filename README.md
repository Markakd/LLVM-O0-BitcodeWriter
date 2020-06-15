# LLVM-O0-BitcodeWriter
patch for LLVM to generate O0 bitcode when compiling

https://github.com/llvm/llvm-project/tree/5521236a18074584542b81fd680158d89a845fca

# Steps

### patch
```bash
git clone https://github.com/llvm/llvm-project
path < WriteBitcode.patch
```

### build clang
```bash
mkdir build && cd build
cmake -DLLVM_ENABLE_PROJECTS=clang -DCMAKE_BUILD_TYPE=Release  -G "Unix Makefiles" ../llvm
make -j$(nproc)
```
