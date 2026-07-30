# 001 — Sequence: Auth

```plantuml
@startuml
title Auth Sequence 1
actor User as A
participant "Auth Service" as S
database "GitHubEdit" as DB
A -> S : authRequest()
activate S
S -> DB : query Account

