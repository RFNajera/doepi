# DoEpi (CDC) — Web Revival

This repository contains a browser-based revival of **DoEpi**, a DOS-era epidemiology training program originally developed by the CDC.

The goal of this project is preservation and accessibility. The original training program now runs inside a modern web browser using WebAssembly (via js-dos), without requiring DOSBox or any additional installation.

This is the original program environment, preserved and made portable.

---

# What This Repository Contains

* The original DoEpi DOS training program
* A `.jsdos` bundle compatible with modern browsers
* An `index.html` launcher page
* All required emulator assets

No installation of DOS software is required.

---

# System Requirements

* A modern browser (Chrome, Edge, Firefox, Safari)
* Keyboard input enabled
* Local file access or a simple local web server

---

# Getting Started

## Option 1 — Download and Open Directly

1. Click the green **Code** button on GitHub.
2. Select **Download ZIP**.
3. Extract the ZIP file to your computer.
4. Open the extracted folder.
5. Double-click `index.html`.

The emulator should load automatically.

> If nothing appears or the emulator fails to start, use Option 2 below.

---

## Option 2 — Run Using a Local Web Server (Recommended)

Some browsers restrict features when opening files directly.
Running a local server avoids this issue.

### macOS / Linux

Open Terminal inside the repository folder and run:

```bash
python3 -m http.server 8000
```

Then open:

```
http://localhost:8000
```

---

### Windows (PowerShell)

Open PowerShell inside the repository folder and run:

```powershell
py -m http.server 8000
```

Then open:

```
http://localhost:8000
```

---

# Running DoEpi

When the emulator loads:

1. You will be prompted to "Select jsdos/zip file to start..."
2. Upload the .jdos file you downloaded as part of the repository.
3. You will be prompted to start the emulation or enter a key to maintain your progress. (Go to https://v8.js-dos.com/key/ to get a key so you can save your progress, if you wish.)
5. Click inside the emulator window to activate keyboard input.
6. You will see a DOS prompt.
7. At the `C:\>` prompt, type `cd doepi`, which will take you to the DOEPI directory.
8. Follow the instructions below...

---

## Step 1 — Extract the Program Files

Run each of the four executables:

```
DOEPI1.EXE
DOEPI2.EXE
DOEPI3.EXE
DOEPI4.EXE
```

These files simulate the original floppy disk installation process and unpack the full program.

---

## Step 2 — Run the Installer

After extracting all four executables, run:

```
INSTALL.EXE
```
Choose which version you want to install:
* Full Installation (Instructor's Module & All Exercises)
* Students' Version (Exercises Only)
* Intro to Epidemiology and Epi Info (3 Outbreaks & Research Study)
* Epi Info and Surveillance (4 Surveillance Exercises)
* Advanced Epi Info (4 Advanced Epi Info Exercises)

If prompted for Disk 2, Disk 3, or Disk 4, simply press **Enter**. (Because all executable files are already present in the same directory, the installer will proceed successfully.)

---

## Step 3 — Launch the Training Program

Once installation is complete:
* You will see a blue screen. Choose `3. Will run from DOS; do not install an icon` to go back to the terminal.
* Type `DOEPI` at the command (`C:\DOEPI>`) prompt.

The DoEpi training program should now start. **If you did not get a key, you will lose all progress and have to repeat the procedure again next time.**

---

# Emulator Controls

* Click inside the emulator window to enable typing.
* Press `Esc` to release the mouse pointer.
* Use the emulator menu for full-screen mode if needed.
* If the screen appears frozen, refresh the browser and restart.

---

# A Video of the Installation Process Will Be Uploaded Here Soon

* [Click here to see a video of the installation process.](https://share.zight.com/8LuzRlOE)

---

# Instructor Notes

This project preserves the original DOS-based interface.

It does not modify or modernize the training software itself. Instead, it provides browser-based access for:

* Historical exploration
* Teaching epidemiology fundamentals
* Demonstrating early computer-assisted public health training
* Comparing past and present analytic tools

For instructional use, consider pairing the exercises with modern analytic tools such as R, Epi Info, or other statistical software.

---

# License

The original DoEpi materials were released as public domain training materials.
This repository preserves and distributes them in that spirit.

---

# Acknowledgment

DoEpi was developed as a CDC training tool to teach epidemiologic methods using interactive, computer-based exercises.

This repository makes that original experience accessible to modern learners.
