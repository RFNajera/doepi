#DoEpi (CDC) — Web Revival

This repository contains a browser-based revival of DoEpi, a DOS-era epidemiology training program originally developed by CDC.

The goal is preservation and accessibility: you can now run the original program in a modern web browser using WebAssembly (via js-dos), without installing DOSBox or any additional software.

This project preserves the original training environment while making it accessible for teaching, demonstration, and historical exploration.

##What This Is

-The original DoEpi DOS program
-Packaged into a .jsdos bundle
-Runnable directly in a web browser
-No installation required
-Works on macOS, Windows, and Linux

This is the original program, not a rewrite.

##How to Use
###Option 1 — Run Directly from GitHub (Simple)
If you are viewing this repository on GitHub:
1. Click Code
2. Select Download ZIP
3. Extract the ZIP file to your computer
4. Open the extracted folder
5. Double-click index.html

Your browser should open the emulator automatically.

###Option 2 — Run with a Local Web Server (Recommended)

Some browsers block certain features when opening files directly.
If index.html does not load properly, use a simple local server.

macOS / Linux

Open Terminal in the repository folder and run:

python3 -m http.server 8000

Then open:

http://localhost:8000
Windows (PowerShell)
py -m http.server 8000

Then open:

http://localhost:8000
Starting the Training

When the emulator loads:

Click inside the emulator window to activate keyboard input.

If prompted to run installation disks, proceed as follows.

Extract the Program Files

In the DOS prompt, run each of the four executables:

DOEPI1.EXE
DOEPI2.EXE
DOEPI3.EXE
DOEPI4.EXE

These extract the program contents into the working directory.

After running all four:

INSTALL.EXE

If prompted for Disk 2, Disk 3, or Disk 4, simply press Enter.
Because all executables are present in the same directory, the installer will proceed correctly.

Launch DoEpi

After installation completes:

CD \DOEPI
DOEPI.EXE

The training program should now start.

Controls

Click inside the emulator window to enable typing.

Press Esc to release the mouse.

Use the emulator menu for fullscreen mode if desired.

Notes for Instructors

This repository preserves the original DOS interface.
It does not modernize the software itself.

For teaching purposes, consider:

Providing contextual guidance outside the emulator

Pairing exercises with modern analytic tools (R, Epi Info, etc.)

Using this as a historical comparison tool

License

The original DoEpi materials were released as public domain training materials.
This repository preserves and distributes them in that spirit.
