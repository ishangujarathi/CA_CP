To run the code we first need to build tour.js file from tour.c file using following command: `emcc -std=c11 -Weverything -Werror -Wno-unused-function -Wno-language-extension-token -O2 -s ASSERTIONS=1 -s EXPORTED_FUNCTIONS='["_getNextPointSerialize"]' -s EXTRA_EXPORTED_RUNTIME_METHODS='["ccall","cwrap"]' -o tour.js src/tour.c` (without the backticks)

After that run index.html and code runs
