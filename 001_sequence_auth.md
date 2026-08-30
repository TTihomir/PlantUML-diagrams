# 001 — Sequence: Auth

```plantuml
@startuml
title Auth Sequence 166
actor User as A
participant "Auth Service" as S
database "GitHubEdit" as DB
A -> S : authRequest()
activate S
S -> DB : query Account
DB --> S : result
S --> A : 4000000 OK
deactivate S
note right of S : handled by Guest
@enduml
```
