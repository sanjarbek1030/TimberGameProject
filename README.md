Timber - 2D C++ Game with SFML
A fast-paced 2D arcade game built in C++ using the Simple and Fast Multimedia Library (SFML).

🛠️ Prerequisites & Downloads
Before setting up the project, download and install the following:

Visual Studio 2026 (or VS 2022/2019) with the Desktop development with C++ workload installed.

SFML 2.6.x (Visual C++ 32-bit / x86)

Download SFML 2.6.0+ (Visual C++ 32-bit) from the official SFML website.

Extract the downloaded ZIP package to C:\SFML (or your preferred path).

📥 How to Clone or Pull the Repository
Open your terminal or command prompt and run:

Bash
git clone https://github.com/your-username/Timber.git
cd Timber
If you already have the repository cloned and want to fetch the latest updates:

Bash
git pull origin main
⚙️ Visual Studio Configuration Guide
Open the Project

Double-click Timber.sln to open the project in Visual Studio.

Set the Target Configuration

On the top toolbar next to the Play / Debug button, set the configuration dropdowns to Debug and x86 (or Win32).

Configure Include & Library Directories

Right-click the Timber project in Solution Explorer and choose Properties (Alt + F7).

Set Configuration to All Configurations and Platform to Win32 (or x86).

Navigate to C/C++ -> General -> Additional Include Directories:

Plaintext
C:\SFML\include
Navigate to Linker -> General -> Additional Library Directories:

Plaintext
C:\SFML\lib
Link SFML Dependencies

Navigate to Linker -> Input -> Additional Dependencies and add:

Plaintext
sfml-graphics-d.lib
sfml-window-d.lib
sfml-system-d.lib
sfml-audio-d.lib
Place Assets & Dynamic Link Libraries (DLLs)

Make sure the following folders and files exist in your project working directory (where Timber.vcxproj is located):

graphics/

sound/

fonts/

sfml-graphics-d-2.dll (copied from C:\SFML\bin)

sfml-window-d-2.dll (copied from C:\SFML\bin)

sfml-system-d-2.dll (copied from C:\SFML\bin)

sfml-audio-d-2.dll (copied from C:\SFML\bin)

🚀 How to Run the Game
Inside Visual Studio
Press F5 to run with debugging, or Ctrl + F5 to run without debugging.

Standalone Executable (Outside Visual Studio)
Switch your configuration to Release (x86) and build the project (Ctrl + Shift + B).

Navigate to your output directory (Timber/Release).

Copy the non-debug SFML DLLs from C:\SFML\bin into this folder:

sfml-graphics-2.dll

sfml-window-2.dll

sfml-system-2.dll

sfml-audio-2.dll

Copy your graphics/, sound/, and fonts/ folders into the same directory.

Launch Timber.exe directly.
