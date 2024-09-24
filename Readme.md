This Repo consists of my progress while learning Opengl

## Note

1. This repo is created on wayland display system(hyprland) and glfw has issues with it so adjustments are made in its CMakeLists.txt such that it works with out any issue

2. I use neovim as my editor and clang as my LSP which requires me to generate compilecommands.json file which enables code suggestion from external libraris (its included in the CMakeLists.txt)

3. Glad Doesn't work well with clang lsp to provide completions for Opengl functions since it uses Macros so as replacement I use glew(its hardly a 3 line change)

### TIP

Clang format can sometimes change the order of include files in your files , to avoid it use comments between them like

```cpp
#include <glew/glew.h>
// #include <glad/glad.h>
#include <GLFW/glfw3.h>
```
