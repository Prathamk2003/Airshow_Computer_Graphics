# Airshow_Computer_Graphics

## ✨ Features
- Multiple Airplanes: Several airplanes perform synchronized maneuvers.
- Tricolor Smoke Trails: Airplanes emit smoke in saffron, white, and green colors, forming the Indian flag's tricolor in the sky.
- Dynamic Camera: The camera follows the lead airplane, providing an immersive experience.
- Interactive Controls: Control the airplane's movement and switch between different views and menus.
- Detailed Environment: Includes a ground, bridge structures, and clouds to enhance the scene.
- Reflections: The water surface features reflections of the surrounding environment.
- User-Friendly Interface: An initial menu system guides the user through the application, including help and introduction sections.

## 🚀 Getting Started
These instructions will get you a copy of the project up and running on your local machine.

Prerequisites

To compile and run this OpenGL project, you'll need:
- GCC (GNU Compiler Collection): A C compiler.
- FreeGLUT / GLUT Development Libraries: OpenGL Utility Toolkit.

For Ubuntu/Debian:
```Bash
sudo apt-get update
sudo apt-get install build-essential libglu1-mesa-dev freeglut3-dev
```

For macOS:
You typically have clang (an Apple-specific GCC derivative) pre-installed. You'll need to install freeglut via Homebrew:
```Bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install freeglut
```

For Windows:
You'll need to set up a C/C++ development environment. MinGW-w64 with MSYS2 is a popular choice:

Download MSYS2: Go to https://www.msys2.org/ and follow the installation instructions.

Install MinGW-w64 and Msys2-devel:
```Bash
pacman -Syu
pacman -Su
pacman -S mingw-w64-x86_64-gcc mingw-w64-x86_64-freeglut mingw-w64-x86_64-libgl
```
Ensure you run these commands within the MSYS2 MinGW 64-bit shell.

## Installation
1. Clone the repository (or download airshow.c):
```Bash
git clone https://github.com/yourusername/airshow-simulation.git
cd airshow-simulation
```
(If you only have the airshow.c file, simply navigate to its directory.)

2. Compile the source code:
Open your terminal or command prompt, navigate to the directory where airshow.c is saved, and run the following command:
```Bash
gcc airshow.c -o airshow -lGL -lGLU -lglut -lm
```
- gcc airshow.c: Compiles the airshow.c source file.
- -o airshow: Specifies the output executable name as airshow.
- -lGL -lGLU -lglut: Links the OpenGL, GLU, and GLUT libraries.
- -lm: Links the math library (for sin, cos, etc.).

## Running the Application
After successful compilation, run the executable:
```Bash
./airshow
```

On Windows, you might just run:
```Bash\
airshow.exe
```

## 🎮 Controls
The simulation features an interactive menu system. Once the airshow begins (after selecting "PROCEED" from the main menu), you can use the following controls:
- Mouse Left Click: Initiates rotational translation (airplane curves).
- Mouse Right Click: Stops rotational translation.
- U / u: Move the airplanes upwards.
- D / d: Move the airplanes downwards.
- P / p: Pause the airplane movement.
- S / s: Start/Resume the airplane movement.
- R / r: Reset the airshow to its initial state.
- B / b: Go back to the previous menu.
- H / h: Go to the main menu (Home).
- Q / q: Quit the application.
