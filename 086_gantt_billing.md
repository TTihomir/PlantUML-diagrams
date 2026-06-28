# 086 — Gantt: Billing

```plantuml
@startgantt
title Billing Roadmap 86
[Design] lasts 5 days
[Build] lasts 10 days
[Build] starts at [Design]'s end
[Test] lasts 4 days
[Test] starts at [Build]'s end
[Release] lasts 1 day
[Release] starts at [Test]'s end
@endgantt
```
