<div align="center">

<img src="dependencies/header.png" width="50%" alt="Header">

## *Rock Band 1 Deluxe* is a light quality-of-life improvement mod for RPCS3 and Xbox 360.

</div>
<br/>

# ✍️ What You'll Need

### Playing *Rock Band 1 Deluxe* requires these things:

- **A vanilla copy of Rock Band 1** for PS3 or Xbox 360 that you can extract onto your PC. The **USA** version is required.
    - (PS3: `BLUS30050`, 360: `45410829`)
- For Console: A **modded/hacked Xbox 360** and a way to transfer files to it. RB1DX currently does not work on PS3 hardware.
- For Emulator: A PC capable of running RPCS3.

<br/>

# 📥 Downloads

![last updated:](https://img.shields.io/github/last-commit/hmxmilohax/rock-band-1-deluxe?label=last%20updated%3A)

### 📥 [RPCS3](https://nightly.link/hmxmilohax/rock-band-1-deluxe/workflows/build/main/RB1DX-PS3.zip)

### 📥 [Xbox 360](https://nightly.link/hmxmilohax/rock-band-1-deluxe/workflows/build/main/RB1DX-Xbox.zip)

> NOTE: *Rock Band 1 Deluxe* currently does not work on PS3 hardware.

<br/>

# 📩 How to Install

### Select your Platform of Choice

  - [RPCS3](#-installing-on-rpcs3)
  - [Xbox 360](#-installing-on-xbox-360)
<br/>

## 📩 Installing on [RPCS3](https://rpcs3.net/)

> If you have a legacy RB1DX install (before November 2023), please re-dump your game before continuing.

* **Install your North American copy of Rock Band 1** (BLUS30050) through the emulator. The [**official RPCS3 site covers this nicely**](https://rpcs3.net/quickstart).

### Download [**Rock Band 1 Deluxe**](https://nightly.link/hmxmilohax/rock-band-1-deluxe/workflows/build/main/RB1DX-PS3.zip) if you haven't already. 
* Extract the `.zip` file.
* **Drag and drop the `.pkg` file on top of the main RPCS3 window** to install it.
* Select `Yes` to confirm.

### ✅ *Rock Band 1 Deluxe is now installed and ready to play!*

<br/>

***Sidenote:*** *we recommend* ***enabling `Write Color Buffers`*** *for Rock Band 1 to prevent any character model issues.*

<br/>

## 📩 Installing on Xbox 360

> RB1DX requires a modded Xbox 360 console (RGH/JTAG) in order to run.

### Install your copy of Rock Band 1 to the console's hard drive. This step is required.
* We recommend that you rename its default.xex to default_vanilla.xex, just as a backup in case you ever want to go back to vanilla.
### Download [**Rock Band 1 Deluxe**](https://nightly.link/hmxmilohax/rock-band-1-deluxe/workflows/build/main/RB1DX-Xbox.zip) if you haven't already
* Extract the .zip file.
* Copy the contents of it to where you have Rock Band 1 installed.
    * You can do this via FTP or by putting the files on a USB drive and copying them using Aurora's file manager.
* Select Yes to overwrite the files if it asks you to.

### Before you launch the game for the first time, we recommend that you...

* Disable any title updates you may have for Rock Band 1 in Aurora.
    * Rock Band 1 Deluxe rolls the latest one into its installation.
    * If you've never played Rock Band 1 on your console, you don't need to do this.
* Clear your song cache.
    * In the dashboard, navigate to System Settings > Storage > Rock Band and delete the song cache.
* Clear your system cache.
    * In the dashboard, navigate to System Settings > Storage and press Y to clear the system cache.
    * If you've never played Rock Band 1 on your console, you don't need to do this.

### ✅ *Rock Band 1 Deluxe is now installed and ready to play!*

<br/>

# 🔨 Building (Advanced)

### Installing Python (Required)

* Head to the [**Python downloads**](https://www.python.org/downloads/), download and install Python (version 3.9 or later).
  * ***Select "Add python.exe to PATH"*** on the installer.

![Python PATH](dependencies/images/pythonpath.png)

### Initializing the Repo

* Go to the **[Releases](https://github.com/hmxmilohax/rock-band-1-deluxe/releases)** of this repo and **download `_init_repo.py`**.
  * Make a new **empty** folder, **put `_init_repo.py` in the folder, and run it**. This will pull the repo down for you and make sure you're completely up to date. **This will take some time.**

### ***The folder should look like this once it's done:***

![Repo Folder](dependencies/images/repofolder.png)

### ✅ ***The Rock Band 1 Deluxe repo is now set up!***

From here, you can make any personal modifications to the game or build it yourself.

* Navigate to `windows_bats` if you're on Windows or `user_scripts` if you're on Linux.
  * Run the `build_` script for your platform of choice to build *Rock Band 1 Deluxe*.
  * Built contents will be in the `_build` folder on the root of the repo.

<br/>

# 🖥️ Dependencies

[Git for Windows](https://gitforwindows.org/) - CLI application to allow auto updating Deluxe repo files

[Dot Net 6.0 Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime) - Needed to run ArkHelper

[Python](https://www.python.org/downloads/) - For user script functionality (NOTE: 3.9 or newer is highly recommended!)

[Mackiloha](https://github.com/PikminGuts92/Mackiloha) - ArkHelper for building Deluxe - SuperFreq for building .bmp_xbox highway images

[swap_rb_art_bytes.py](https://github.com/PikminGuts92/re-notes/blob/master/scripts/swap_rb_art_bytes.py) - Python script for converting Xbox images to PS3

[dtab](https://github.com/mtolly/dtab) - For serializing `.dtb` script files
