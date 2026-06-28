# 054 — Component: Analytics

```plantuml
@startuml
title Analytics Components 54
package "Analytics" {
  [Web UI] as UI
  [Analytics API] as API
  [Analytics Service] as SVC
  database "AnalyticsDB" as DB
  [Cache] as C
}
UI --> API
API --> SVC
SVC --> DB
SVC --> C
@enduml
```
