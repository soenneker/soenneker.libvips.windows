[![](https://img.shields.io/nuget/v/soenneker.libvips.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.windows/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.windows/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.windows/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libvips.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.windows/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.windows/codeql.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.windows/actions/workflows/codeql.yml)

# ![](https://user-images.githubusercontent.com/4441470/224455560-91ed3ee7-f510-4041-a8d2-3fc093025112.png) Soenneker.Libvips.Windows
### Provides the native libvips shared library for Windows x64.

## Installation

```
dotnet add package Soenneker.Libvips.Windows
```

The package places `libvips-42.dll` under `runtimes/win-x64/native`, so .NET selects and copies it for Windows x64 applications automatically.

The binary comes from [kleisauke/libvips-packaging](https://github.com/kleisauke/libvips-packaging). Third-party notices and exact component versions are included in the package.
