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

error: ""ABRA02486\r\nHFDTE301217\r\nHFFXA100\r\nHFPLTPILOT:..."" (line 1, column 1):
unexpected "A"
expecting xml declaration, comment, processing instruction, "<!DOCTYPE" or "<"


error: ""AXCGAventura  3.0|C17B-20520095\r\nHFDTE301217\r..."" (line 1, column 1):
unexpected "A"
expecting xml declaration, comment, processing instruction, "<!DOCTYPE" or "<"
```
