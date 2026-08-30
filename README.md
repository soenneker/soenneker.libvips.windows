[![](https://img.shields.io/nuget/v/soenneker.libvips.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.windows/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.windows/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.windows/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.windows/publish-package.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.windows/actions/workflows/publish-package.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libvips.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.windows/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.windows/codeql.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.windows/actions/workflows/codeql.yml)

# Soenneker.Libvips.Windows

The libvips command-line distribution packaged for Windows x64 .NET applications.

## Install

```bash
dotnet add package Soenneker.Libvips.Windows
```

## Runtime files

The package copies `bin/vips.exe`, `bin/vipsheader.exe`, and their required runtime files beneath the application output directory:

```text
Resources/win-x64/libvips/
```

Resolve that directory from `AppContext.BaseDirectory`; do not depend on the process working directory. This package contains Windows x64 assets only and does not select a distribution for other operating systems or architectures.

Most applications should reference `Soenneker.Libvips.Util`, which selects and invokes the matching platform tool. Reference this package directly when you need the native distribution without the managed wrapper.

The distribution comes from [libvips/build-win64-mxe](https://github.com/libvips/build-win64-mxe).
