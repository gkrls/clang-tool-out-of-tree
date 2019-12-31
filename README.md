# clang-tool-out-of-tree

The Syntax-Checker Tool from [here](https://clang.llvm.org/docs/LibASTMatchersTutorial.html) but built out-of-tree!

Requires `$LLVM_HOME` to be defined and point to a valid LLVM install directory wit the following structure:
```
$LLVM_HOME
|_bin
|_include
|_lib
  |_clang
  |_10.0.0
    |_include
    |_lib
    |_share
|_libexec
|_share
```

Tested on **LLVM 10**.

## Usage:

Clone anywhere:
```
$ git clone https://github.com/gkarlos/clang-tool-out-of-tree
```

Build:
```
cd clang-tool-out-of-tree
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
