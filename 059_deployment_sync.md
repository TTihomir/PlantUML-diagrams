# 059 — Deployment: Sync

```plantuml
@startuml
title Sync Deployment 59
node "Load Balancer" as LB
node "App Server" {
  artifact "sync-app.war" as APP
}
node "DB Server" {
  database "SyncDB" as DB
}
cloud "CDN" as CDN
LB --> APP
APP --> DB
CDN --> LB
@enduml
```
