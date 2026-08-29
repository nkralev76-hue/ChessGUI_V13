# Ferz — CMD Chess GUI (v13)

Малка графична среда за игра на шах с SDL2, с поддръжка на два UCI
двигателя едновременно, вграден двигател (StrongEngine), opening book,
анализ на ходове, ponder и теми.

## Компилация (Windows, MinGW64)

```bat
gcc -O3 -march=native -mpopcnt -mavx2 -DUSE_BOOK ^
    -o chess_gui_v13.exe chess_gui_v13.c ^
    -lSDL2 -lSDL2_image -lm -lcomdlg32
```

Нужни са `SDL2.dll`, `SDL2_image.dll`, `libpng16-16.dll`, `zlib1.dll`
(в папката с .exe) и папката `pieces/` с фигурите. `book.h` е нужен
само по време на компилация.

## Лиценз

MIT — свободен за ползване, промяна и разпространение. Виж `LICENSE`.
