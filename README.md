## Overview
This project is a C/C++ application that generates and displays a fractal triangle using a graphical window. It features interactive controls for zooming, panning, and viewing time metrics.

## Features
- Interactive fractal triangle visualization
- Zoom and pan functionality
- Time metrics displayed on the screen

## Project Structure
```
Gui_Triangle_Fractal/
├── build/              # Compiled executable files
├── src/
│   ├── Main.c          # Entry point
│   └── *.h             # Header files used by Main.c
├── Makefile.linux      # Linux build configuration
├── Makefile.windows    # Windows build configuration
├── Makefile.wine       # Wine build configuration
├── Makefile.web        # Web assembly build configuration
└── README.md           # This file
└── LICENSE             # License file
```

### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools
- Libraries: X11 for GUI rendering, PNG and JPEG for image handling

## Build & Run
### Linux
To build the project on Linux:
```sh
cd Gui_Triangle_Fractal/
make -f Makefile.linux all
```
Run the executable with:
```sh
make -f Makefile.linux exe
```

### Windows
To build the project on Windows:
```sh
cd Gui_Triangle_Fractal/
make -f Makefile.windows all
```
Run the executable by double-clicking `Main.exe` or using:
```sh
make -f Makefile.windows exe
```

### Web Assembly (Emscripten)
To build for web assembly:
```sh
cd Gui_Triangle_Fractal/
make -f Makefile.web all
```
Serve the output with an HTTP server, and open `index.html` in your browser.

### Wine (Cross-compile for Windows on Linux)
To cross-compile for Windows using Wine:
```sh
cd Gui_Triangle_Fractal/
make -f Makefile.wine all
```
Run the executable with Wine by double-clicking `Main.exe`.