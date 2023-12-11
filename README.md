# SwiftWorkflows

## Files

-   `buildAndTest.yml`: Checkouts the repository, compiles, and tests (`swift build` and `swift test`) a Swift package on MacOS, Linux, and Windows.
    -   Inputs:
        -   MacOS: A boolean value that indicates if the package should be tested on MacOS.
        -   Linux: A boolean value that indicates if the package should be tested on Linux.
        -   Windows: A boolean value that indicates if the package should be tested on Windows.
-   `generateDocumentation.yml`: Checkouts the repository, compiles the documentation target, builds the `.docc` bundle, transforms it for static hosting, and publishes it to the gh-pages branch.
    -   Inputs:
        -   TargetName: The name of the target to generate documentation for.
        -   DoccBundlePath: The path to the .docc documentation bundle (relative to the root of the repository, for example: Sources/Library/Library.docc)
