# data-ops

## What is this?

This is a collection of Data Ops snippets. It is connected to both Azure DevOps and Github so that concepts can be tested and shared in a more structured way.

## Mermaid test

This has been added to test Mermaid integration in Github and Azure DevOps and has no relevance to anything right now.

### GitGraph Test

```mermaid
---
title: A very simple git diagram
---
gitGraph
  commit
  commit
  branch develop
  commit
  commit
  commit
  checkout main
  merge develop
```

### GitGraph Failed in Azure DevOps

Yeah so that didn't work and furthermore, gitGraph isn't supported by DevOps (boo) only the following:

- Flowchart
- Sequence diagrams
- Gantt charts
- Pie charts
- Requirement diagrams
- State diagrams
- User Journey

### Flowchart Test

So let's try a flowchart:

``` mermaid 
flowchart TD;
    A([Crash land on Dagobah]) --> B[Meet Yoda];
    B --> C[Learn to Use the Force];
    C --> F
    D --> F{Am I ready?}
    F --> |"No"|D[Face Fears in Cave];
    F --> |"No but my friends need me"|G([Leave Dagobah]);
```

### Consolidated Flowchart Test

What is annoying is that they syntax is different for Azure DevOps WHY!?!? Is there a way to consolidate the two? Probably not but here's an attempt...

::: mermaid
``` mermaid 
flowchart TD;
    A([Crash land on Dagobah]) --> B[Meet Yoda];
    B --> C[Learn to Use the Force];
    C --> F
    D --> F{Am I ready?}
    F --> |"No"|D[Face Fears in Cave];
    F --> |"No but my friends need me"|G([Leave Dagobah]);
```
:::