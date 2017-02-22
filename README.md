# WASMSobel
Simple example to show comparing JS/WASM implementations for a Sobel filter
Compile change.c with emscripten using:
emcc -o change.js change.c  -lm -O3 -s WASM=1 -s EXPORTED_FUNCTIONS="['_change']" -s BINARYEN_IMPRECISE=1
