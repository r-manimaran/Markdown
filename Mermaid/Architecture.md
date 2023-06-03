## Architecture
---

```mermaid
---
title: Simple
---

graph TD
    API --> Core{{Core Application}} 
    Infrastructure --> Core
    API --> Infrastructure

```

---
```mermaid
graph TD
    API --> Core
    subgraph Core
        Services --> Domain
    end

    Infrastructure --> Core
    API --> Infrastructure

```

Here TD represents the Top to Down. The other values we can use are
1. TD or TB - Top to bottom or down
1. BT -Bottom to top
1. RL - Right to Left
1. LR - Left to Right

## Different Shapes
---
```mermaid
graph TD
    Rectange
    b{diamond with label}
    c((Circle with Label))
    d>anothershape]
    e[rectangle]
    f(round rectangle)
```
