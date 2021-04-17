# cmakewin32directxsdkimgui

# Packages:
  * imgui 1.82 https://github.com/ocornut/imgui
  * cmake 3.20
  * Viusal Studio 2019
	* Directx SDK
	* Windows Kits 10

# Information:
  Test build for Directx 9-12 in win 64 bit window 10.

  Directx 9-12 work on imgui build.

# Directx checks:
 * Win 32 Directx 9 > pass
 * Win 32 Directx 10 > pass
 * Win 32 Directx 11 > pass
 * Win 32 Directx 12 > pass

# Build:

```bar
mkdir build 
:: Build from that directory so the build files are in one place
cd build
:: config build from CMakeLists.txt
cmake ..
:: build binary app
cmake --build . 
```

# Notes:
 * If Viusal Studio 2019 with Directx SDK that lib are loaded without much need config. As long you pass correct name of lib name in target_link_libraries().

# Credits:
 * https://stackoverflow.com/questions/48955632/finding-direct3d-12-using-cmake
 * https://stackoverflow.com/questions/64789975/finding-directx12-libraries-with-cmake-and-mingw
 * https://gist.github.com/rokups/f771217b2d530d170db5cb1e08e9a8f4
