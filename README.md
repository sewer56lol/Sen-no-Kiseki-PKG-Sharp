# About This Repository
This repository consists of the following components: 

- **PKGLib:** A C# library for handling PKG files .
- **dlang-sencompress:** A high performance library for Sen no Kiseki Compression/Decompression written in the D language.
- **SenCompressSharp:** A C# wrapper for the dlang-sencompress library.
- **PKGToolCmd**: A simple C# commandline utility for extracting and packing of Sen no Kiseki PKG files.

![Exhibit A](https://i.imgur.com/2xd34rH.png)

The compression library component is implemented using the [D Programming Language](https://dlang.org/) and is based off of my own PKG Compressor [dlang-prs](https://github.com/sewer56lol/dlang-prs).

The _PKGLib_ and _SenCompress_ libraries are written in _.NET Standard_ thus can be used with any .NET implementation such as Framework, Core, Xamarin or Mono.

## Documentation

- [PKG File Structure](https://github.com/sewer56lol/Sen-no-Kiseki-PKG-Sharp/blob/master/docs/PKG-File-Structure.md)
- [Compression Explained](https://github.com/sewer56lol/Sen-no-Kiseki-PKG-Sharp/blob/master/docs/Compression-Explained.md)
- [Using the Libraries](https://github.com/sewer56lol/Sen-no-Kiseki-PKG-Sharp/blob/master/docs/Using-The-Libraries.md)

## Compilation Instructions

### Compressor/Decompressor (dlang-sencompress)
- Install the latest version of Visual D: https://github.com/dlang/visuald/releases
- Add the DMD and LDC compilers to your System Environment Variables' PATH (in case they are not added).
![Adding to PATH](https://i.imgur.com/lrMoasL.png)

- Open `Dlang.sln` with Visual Studio.

Note: Successful builds output in `build` directory. where the solution files reside 

### All C# Components (Wrapper, PKG Library, Commandline Util.)
- Install the latest .NET Core 2.X SDK.
- Compile `dlang-sencompress` (see above) for Win32 (x86) and x64.
- Open `CSharp.sln` in Visual Studio and build.

## Adding the libraries to your own project.

Do note that in order to use the actual libraries in your own projects you do not actually need the D compiler. 

Individual precompiled packages are available on NuGet; you will only need the compiler should you choose to contribute to the repository.

For more details see "Using the Libraries".
