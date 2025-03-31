```mermaid
classDiagram
  class PackageMetadata
  <<interface>> PackageMetadata
  PackageMetadata : +string dir
  PackageMetadata : +string noInstall
  PackageMetadata : +PackageManager packageManager
```
