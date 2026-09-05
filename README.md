# Ferz — CMD Chess GUI (v13)

A small graphical chess environment built with SDL2, supporting two UCI
engines simultaneously, a built-in engine (StrongEngine), opening book,
move analysis, ponder and themes.

## Compilation (Windows, MinGW64)

```bat
gcc -O3 -march=native -mpopcnt -mavx2 -DUSE_BOOK ^
    -o chess_gui_v13.exe chess_gui_v13.c ^
    -lSDL2 -lSDL2_image -lm -lcomdlg32
```

Required: `SDL2.dll`, `SDL2_image.dll`, `libpng16-16.dll`, `zlib1.dll`
(in the folder with the .exe) and the `pieces/` folder with the piece
graphics. `book.h` is only needed at compile time.

## License

GPL-3.0 — free to use and modify, but distributed changes must remain
under GPL. See `LICENSE`.