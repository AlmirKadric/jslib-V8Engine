V8 Engine JavaScript libraries
==============================
The purpose of this project is to deliver the V8 engine pre-compiled and pre-packaged for all supported platforms so
that it may be easily dropped into projects for immediate use. It will also come shipped with all the Makefiles used to
compile the libraries so that users may inspect the options used as well as re-compile the libraries if they see it
necessary.

Branching & Tagging
---------------


Compile options
---------------
For performance and immediate production use reasons, all libraries are compiled using the default release options
present in the V8 Makefiles.

Compression
-----------


Platforms
---------
The following platforms are supported by this project and will be present within their respective build folders:
 * Android (ia32 shared, ia32 static, arm shared, arm static, arm64 static)
 * Linux (ia32 shared, ia32 static, x64 shared, x64 static, arm shared, arm static, arm64 shared, arm64 static)
 * MacOSX (ia32 static, x64 shared, x64 static)
 * Windows (ia32 shared, ia32 static, x64 shared, x64 static)

NOTES:
 * Unless jail-broken, IOS does not allow the creation of executable memory pages, on which V8 heavily relies. As such
   the V8 team does not directly support IOS and as a result we will not support IOS for the time being.
 * Similar to IOS, WindowsPhone does not allow the creation of executable memory pages so same result as above.
 * ia32 shared debug build is currently broken for MacOSX on all versions. Since we need both release debug and release
   ia32 shared build is ignored till this is fixed by the V8 team.
 * arm64 shared debug and release is currently broken for Android. arm64 shared build is ignored till this is fixed by
   the V8 team.

Licenses
--------
All original code and scripts within the project are subject to the [MIT license](LICENSE)

All dependencies and their compiled binary files are subject to their original respective licenses as found in their
respective repositories.