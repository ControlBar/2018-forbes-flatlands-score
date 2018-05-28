# Scoring Log

With this repo and [flare-timing](https://github.com/BlockScope/flare-timing)
cloned as siblings the following commands show how to score all tasks at once
for the **Forbes Flatlands 2018** competition.

```
> ../../bin/extract-input --file=forbes2018.fsdb
Extracted 7 tasks from "Forbes Flatlands 2018"
Extracting tasks completed in 1.19 s

> ../../bin/task-length --file=forbes2018.comp-input.yaml
forbes2018.comp-input.yaml
Measuring task lengths completed in 3.91 m

> ../../bin/cross-zone --file=forbes2018.comp-input.yaml
Reading competition from 'forbes2018.comp-input.yaml'
Tracks crossing zones completed in 26.74 s

> ../../bin/tag-zone --file=forbes2018.cross-zone.yaml
Reading zone crossings from 'forbes2018.cross-zone.yaml'
Tagging zones completed in 253.53 ms

> ../../bin/align-time --file=forbes2018.comp-input.yaml
Reading competition from 'forbes2018.comp-input.yaml'
Reading flying time range from 'forbes2018.cross-zone.yaml'
Reading zone tags from 'forbes2018.tag-zone.yaml'
Aligning times completed in 16.61 m

> ../../bin/discard-further --file=forbes2018.comp-input.yaml
Reading competition from 'forbes2018.comp-input.yaml'
Reading task length from 'forbes2018.task-length.yaml'
Reading zone tags from 'forbes2018.tag-zone.yaml'
Filtering times completed in 27.34 s

> ../../bin/mask-track --file=forbes2018.comp-input.yaml
Reading competition from 'forbes2018.comp-input.yaml'
Reading task length from 'forbes2018.task-length.yaml'
Reading flying time range from 'forbes2018.cross-zone.yaml'
Reading zone tags from 'forbes2018.tag-zone.yaml'
Masking tracks completed in 23.05 s

> ../../bin/land-out --file=forbes2018.comp-input.yaml
Reading land outs from 'forbes2018.mask-track.yaml'
Land outs counted for distance difficulty completed in 31.63 ms

> ../../bin/gap-point --file=forbes2018.comp-input.yaml
Reading pilots absent from task from 'forbes2018.comp-input.yaml'
Reading pilots that did not fly from 'forbes2018.cross-zone.yaml'
Reading start and end zone tagging from 'forbes2018.tag-zone.yaml'
Reading masked tracks from 'forbes2018.mask-track.yaml'
Reading distance difficulty from 'forbes2018.land-out.yaml'
Tallying points completed in 314.34 ms
```
