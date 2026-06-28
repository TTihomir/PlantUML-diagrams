# 051 — Component: Cart

```plantuml
@startuml
title Cart Components 51
package "Cart" {
  [Web UI] as UI
  [Cart API] as API
  [Cart Service] as SVC
  database "CartDB" as DB
  [Cache] as C
}
UI --> API
API --> SVC
SVC --> DB
SVC --> C
@enduml
```
