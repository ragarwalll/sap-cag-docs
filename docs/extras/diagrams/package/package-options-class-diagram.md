```mermaid
classDiagram
  class PackageOptions
  <<interface>> PackageOptions
  PackageOptions : +string displayName
  PackageOptions : +PackageType type
  PackageOptions : +Record~string, UserInputMetadata~ metadata
  PackageOptions : +string className
```
