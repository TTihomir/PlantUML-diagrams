# 062 — Deployment: Scheduler

```plantuml
@startuml
title Scheduler Deployment 62
node "Load Balancer" as LB
node "App Server" {
  artifact "scheduler-app.war" as APP
}
node "DB Server" {
  database "SchedulerDB" as DB
}
cloud "CDN" as CDN
LB --> APP
APP --> DB
CDN --> LB
@enduml
```
