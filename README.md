The Syntax-Checker Tool from [here](https://clang.llvm.org/docs/LibASTMatchersTutorial.html) but built out-of-tree!

Requires `$LLVM_HOME` to be defined and point to a valid LLVM install directory

Build:
```
mkdir build
cd build
cmake ..
make
```

Run:
```
./simple-clang-check <your-source-file.cpp>
```

Example:
```
$ ./simple-clang-check ../src/SimpleClangCheck.cpp
Clang Tool Starting...
Syntax OK
```