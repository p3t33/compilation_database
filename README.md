
# compilation database
This repository contains the code accompanying [lsp and cross compilation pitfalls post](https://kobimedrish.com/posts/lsp_and_cross_compilation_pitfalls/)

To compile the code(from the root of directory)

```bash
clang++ app/main.cpp lib/hello_world.cpp -I./lib
```

To compile the code using cmake

``` bash
mkdir build
cd build
cmake ..
cmake --build .
```

To generate compilation database(compile_commands.json)

```bash
cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=ON ..
```



