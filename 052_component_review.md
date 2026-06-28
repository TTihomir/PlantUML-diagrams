# 052 — Component: Review

```plantuml
@startuml
title Review Components 52
package "Review" {
  [Web UI] as UI
  [Review API] as API
  [Review Service] as SVC
  database "ReviewDB" as DB
  [Cache] as C
}
UI --> API
API --> SVC
SVC --> DB
SVC --> C
@enduml
```
