# 089 — Gantt: Catalog

```plantuml
@startgantt
title Catalog Roadmap 89
[Design] lasts 5 days
[Build] lasts 10 days
[Build] starts at [Design]'s end
[Test] lasts 4 days
[Test] starts at [Build]'s end
[Release] lasts 1 day
[Release] starts at [Test]'s end
@endgantt
```
