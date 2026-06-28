# 053 — Component: Recommendation

```plantuml
@startuml
title Recommendation Components 53
package "Recommendation" {
  [Web UI] as UI
  [Recommendation API] as API
  [Recommendation Service] as SVC
  database "RecommendationDB" as DB
  [Cache] as C
}
UI --> API
API --> SVC
SVC --> DB
SVC --> C
@enduml
```
