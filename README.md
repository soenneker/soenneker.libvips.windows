[![](https://img.shields.io/nuget/v/soenneker.libvips.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.windows/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.windows/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.windows/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libvips.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.windows/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.windows/codeql.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.windows/actions/workflows/codeql.yml)

# ![](https://user-images.githubusercontent.com/4441470/224455560-91ed3ee7-f510-4041-a8d2-3fc093025112.png) Soenneker.Libvips.Windows
### Provides a bundled libvips command-line distribution for Windows x64.

## Installation

```
dotnet add package Soenneker.Libvips.Windows
```

The package copies the distribution to `Resources/win-x64/libvips`, including `bin/vips.exe`, `bin/vipsheader.exe`, and their runtime dependencies.

The distribution comes from [libvips/build-win64-mxe](https://github.com/libvips/build-win64-mxe).
