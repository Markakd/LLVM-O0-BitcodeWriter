# LLVM-O0-BitcodeWriter
patch for LLVM to generate O0 bitcode
# Steps

### patch
```bash
git clone https://github.com/llvm/llvm-project
git checkout 5521236a18074584542b81fd680158d89a845fca
path < WriteBitcode.patch
```

### build clang
```bash
mkdir build && cd build
cmake -DLLVM_ENABLE_PROJECTS=clang -DCMAKE_BUILD_TYPE=Release  -G "Unix Makefiles" ../llvm
make -j$(nproc)
```
