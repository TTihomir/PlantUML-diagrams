# 064 — Deployment: Audit

```plantuml
@startuml
title Audit Deployment 64
node "Load Balancer" as LB
node "App Server" {
  artifact "audit-app.war" as APP
}
node "DB Server" {
  database "AuditDB" as DB
}
cloud "CDN" as CDN
LB --> APP
APP --> DB
CDN --> LB
@enduml
```
