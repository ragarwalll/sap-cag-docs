```mermaid
classDiagram
  class PackageType{
      <<enumeration>>
      frontend
      backend
      unknown
  }
  class PackageManager{
    <<enumeration>>
    npm
    yarn
    pnpm
}
```
