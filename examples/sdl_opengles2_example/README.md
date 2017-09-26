
# How to Build

- On Linux and similar Unixes

```
c++ `sdl2-config --cflags` -I ../.. main.cpp imgui_impl_sdl_gles2.cpp ../../imgui*.cpp `sdl2-config --libs` -lGLESv2 -ldl -o sdl2_opengles2_example
```
- Emscripten

```
em++ -O2 -s USE_SDL=2 -I ../.. main.cpp imgui_impl_sdl.cpp ../../imgui*.cpp -o html/index.html
```
