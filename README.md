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

1. Click inside the emulator window to activate keyboard input.
2. You will see a DOS prompt.

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

If prompted for Disk 2, Disk 3, or Disk 4, simply press **Enter**.

Because all executable files are already present in the same directory, the installer will proceed successfully.

---

## Step 3 — Launch the Training Program

Once installation is complete:

```
CD \DOEPI
DOEPI.EXE
```

The DoEpi training program should now start.

---

# Emulator Controls

* Click inside the emulator window to enable typing.
* Press `Esc` to release the mouse pointer.
* Use the emulator menu for fullscreen mode if needed.
* If the screen appears frozen, refresh the browser and restart.

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
