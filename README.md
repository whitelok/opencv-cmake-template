# OpenCV CMake Template

## Build for x86_64
```bash
cd [project root path]
mkdir build
cmake ..
make  -j
```

## Build for Macos M1(arm64)
```bash
cd [project root path]
mkdir build
arch -arm64 cmake -DCMAKE_SYSTEM_PROCESSOR=arm64 -DCMAKE_OSX_ARCHITECTURES=arm64 ..
arch -arm64 make -j
```