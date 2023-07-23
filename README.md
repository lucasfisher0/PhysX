# PhysX

This repo is forked from **[RavEngine/PhysX-Complete](https://github.com/RavEngine/PhysX-Complete)**, and includes additional configurations from [the O3DE fork](https://github.com/o3de/PhysX).

This is to be used for integration into [Unreal Engine](https://github.com/lucasfisher0/UE5X).

# RavEngine/PhysX-Complete
The latest version of NVIDIA PhysX, with modifications to make it compile with CMake on more platforms.
Developed for use in [RavEngine](https://github.com/RavEngine/RavEngine). 

## How to use:
```cmake
add_subdirectory(physx-complete)

target_include_directories(your-app
	PUBLIC 
	"physx-complete/physx/physx/include/" 
	"physx-complete/physx/pxshared/include/" 
	"physx-complete/physx/physx/snippets/"
)

target_link_libraries(your-app PRIVATE 
	"PhysXExtensions"
	"PhysX"
	"PhysXPvdSDK"
	"PhysXVehicle"
	"PhysXCharacterKinematic"
	"PhysXCooking"
	"PhysXCommon"
	"PhysXFoundation"
	"PhysXTask"
	"FastXml"
	"LowLevel"
	"LowLevelAABB"
	"LowLevelDynamics"
	"SceneQuery"
	"SimulationController"
)
```

**Supported Platforms:**
- macOS (Intel and Apple Silicon)
- Windows Win32
- Windows UWP
- Linux
- iOS 
- AppleTV 
- WebAssembly / Emscripten


### Current Version
- PhysX 5.1.2 as of Dec 12, 2022 (No Blast yet)

### Contributing
Contributions are welcome. Please submit Issues if you find problems, and Pull Requests to address issues. If the problem is
within PhysX itself, submit your issues and pull requests there. 
