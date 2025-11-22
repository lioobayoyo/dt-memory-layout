# Building instructions

## Windows 

### Install Git for Windows

See existing guides all over the internet, for instance here:
https://github.com/Dwarf-Therapist/Dwarf-Therapist/blob/master/BUILDING.md#visual-studio-version (section 3.)

### Get source code

From a terminal, in a folder where you want to put the source code, including the external library libdfs in git submodule:

```
git clone https://github.com/cvuchener/dt-memory-layout
cd dt-memory-layout
git submodule update --init --recursive
```

### Install Visual Studio

Get latest Visual Studio 2026 Community installer here (free):
https://visualstudio.microsoft.com/downloads/

Select "Desktop development with C++" (tab installer workloads).
  
Make sure the following are included (tab "Individual Components"):

  * vcpkg package manager
  * C++ CMake tools for Windows
 
 ### Build
 
 In VS2026 launcher, choose "Open folder", open the `dt-memory-layout/` source code folder.
 
 Wait a moment for Visual Studio to refresh packages cache.
 
 When done, select menu "Build > Build All".
 
 The executable is in `dt-memory-layout\out\build\x64-Debug` folder.
 