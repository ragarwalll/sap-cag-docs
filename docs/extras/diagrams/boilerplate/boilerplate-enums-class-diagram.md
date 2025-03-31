```mermaid
classDiagram
  class AvailablePackagesMap{
      <<enumeration>>
      ui5
      react
      springboot
      nodejs
  }
  class BoilerplateFlags
  <<interface>> BoilerplateFlags
  BoilerplateFlags : +boolean noGit
  BoilerplateFlags : +boolean noInstall
  BoilerplateFlags : +boolean default
```
