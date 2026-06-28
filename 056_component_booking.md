# 056 — Component: Booking

```plantuml
@startuml
title Booking Components 56
package "Booking" {
  [Web UI] as UI
  [Booking API] as API
  [Booking Service] as SVC
  database "BookingDB" as DB
  [Cache] as C
}
UI --> API
API --> SVC
SVC --> DB
SVC --> C
@enduml
```
