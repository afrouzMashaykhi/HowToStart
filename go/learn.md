## go.mod
The go command resolves imports by using the specific dependency module versions listed in `go.mod`. When it encounters an import of a package not provided by any module in `go.mod`, the go command automatically looks up the module containing that package and adds it to `go.mod`, using the latest version. (“Latest” is defined as the latest tagged stable (non-prerelease) version, or else the latest tagged prerelease version, or else the latest untagged version.)
The go mod tidy command cleans up these unused dependencies
## go.sum
In addition to `go.mod`, the go command maintains a file named `go.sum` containing the expected cryptographic hashes of the content of specific module versions
