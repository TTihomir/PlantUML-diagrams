# 057 — Component: Chat

```plantuml
@startuml
title Chat Components 57
package "Chat" {
  [Web UI] as UI
  [Chat API] as API
  [Chat Service] as SVC
  database "ChatDB" as DB
  [Cache] as C
}
UI --> API
API --> SVC
SVC --> DB
SVC --> C
@enduml
```
