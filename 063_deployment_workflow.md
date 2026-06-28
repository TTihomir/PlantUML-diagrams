# 063 — Deployment: Workflow

```plantuml
@startuml
title Workflow Deployment 63
node "Load Balancer" as LB
node "App Server" {
  artifact "workflow-app.war" as APP
}
node "DB Server" {
  database "WorkflowDB" as DB
}
cloud "CDN" as CDN
LB --> APP
APP --> DB
CDN --> LB
@enduml
```
