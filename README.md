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

* **Install your North American copy of Rock Band 1** through the emulator. The [**official RPCS3 site covers this nicely**](https://rpcs3.net/quickstart).
  * Remember, **Rock Band 1 needs to be** ***BLUS30050***. RPCS3 will tell you this in the game selection GUI under the `Serial` column.

<img src="dependencies/images/serial.png" alt="Serial">

* Download [**Rock Band 1 Deluxe**](hhttps://nightly.link/hmxmilohax/rock-band-1-deluxe/workflows/build/main/RB1DX-PS3.zip). 
  * Extract the zip and **drag and drop the `.pkg` file on top of the main RPCS3 window** to install it.
  * Select `Yes` to confirm.

<img src="dependencies/images/rpcs3_dxpkg.png" alt="RPCS3 DX PKG">

### ✅ ***Rock Band 1 Deluxe is now installed!***

<br/>

***Sidenote:*** *we recommend* ***enabling `Write Color Buffers`*** *for Rock Band 1 to prevent any character model issues.*

![Custom Configuration](dependencies/images/customconfig.png)
![GPU Tab](dependencies/images/gputab.png)
![Write Color Buffers](dependencies/images/writecolorbuffers.png)

<br/>

## 📩 Installing on Xbox 360

**NOTE: You WILL need a HACKED/MODDED (RGH or JTAG) Xbox 360 in order to play this mod on console. We hope this is clear.**

* **Install your vanilla copy of Rock Band 1** to your console's hard drive.
  * In case anything goes wrong, we recommend that you **rename `default.xex` to `default_vanilla.xex`**.

* **Disable updates** for Rock Band 1 in Aurora. *Rock Band 1 Deluxe* rolls the latest one into its base installation.

* Download [**Rock Band 1 Deluxe**](https://nightly.link/hmxmilohax/rock-band-1-deluxe/workflows/build/main/RB1DX-Xbox.zip). 
  * **Copy the contents of it to where your copy of Rock Band 1 is installed** (we recommend using FTP to do so).
  * Select `Yes` to overwrite the files if it asks you to.

### ✅ ***Rock Band 1 Deluxe is now installed!***

<br/>

***Sidenote:*** We also recommend **clearing your song cache**, as well as your **system cache**.
* *To clear your **song cache**, navigate to `System Settings > Storage > Rock Band 1` and delete the song cache.*
* *To clear your **system cache**, navigate to `System Settings > Storage` and press `Y` to clear the system cache.*

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
