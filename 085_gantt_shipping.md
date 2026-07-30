# 085 — Gantt: Shipping

```plantuml
@startgantt
title Shipping Roadmap 85
[Design] lasts 5 days
[Build] lasts 10 days
[Build] starts at [Design]'s end
[Test] lasts 4 days
[Test] starts at [Build]'s end
[Release] lasts 1 day
[Release] starts at [Test]'s end
@endgantt
```
