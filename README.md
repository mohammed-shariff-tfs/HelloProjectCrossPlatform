# HelloProjectCrossPlatform

A simple C++ project configured with CMake.

## Project Structure

```
HelloProjectCrossPlatform/
├── include/           # Header files
├── src/               # Source files (*.cpp)
├── CMakeLists.txt     # CMake build configuration
├── commands.txt       # Helpful build commands
└── README.md          # Project documentation
```

## Requirements

- CMake >= 3.10
- A C++17-compatible compiler (GCC, Clang, or MSVC)

## Build Instructions

### Unix/Linux/macOS

```sh
# Create and enter the build directory
mkdir build
cd build

# Configure the project (default is Release)
cmake ..

# Build the project
cmake --build .

# Run the application
./ProjectApplication

# Clean the build
cmake --build . --target clean
```

### Windows (Debug and Release Builds)

```bat
:: Configure and build Debug version
cmake -S . -B build -DCMAKE_BUILD_TYPE=Debug
cmake --build build --config Debug

:: Configure and build Release version
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build --config Release
```

## Build Features

- C++17 standard enforced
- Compiler warnings enabled:
  - **MSVC**: `/W4 /permissive-`
  - **GCC/Clang**: `-Wall -Wextra -pedantic`
- Definitions for build types:
  - `DEBUG_BUILD` (for Debug)
  - `RELEASE_BUILD` (for Release)
- Custom output directories for Debug and Release builds

## License

Add your license information here.

---

Happy coding! 🎉

