# 058 — Component: Upload

```plantuml
@startuml
title Upload Components 58
package "Upload" {
  [Web UI] as UI
  [Upload API] as API
  [Upload Service] as SVC
  database "UploadDB" as DB
  [Cache] as C
}
UI --> API
API --> SVC
SVC --> DB
SVC --> C
@enduml
```
