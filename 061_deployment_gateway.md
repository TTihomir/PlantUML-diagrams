# 061 — Deployment: Gateway

```plantuml
@startuml
title Gateway Deployment 61
node "Load Balancer" as LB
node "App Server" {
  artifact "gateway-app.war" as APP
}
node "DB Server" {
  database "GatewayDB" as DB
}
cloud "CDN" as CDN
LB --> APP
APP --> DB
CDN --> LB
@enduml
```
