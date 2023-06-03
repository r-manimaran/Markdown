## FlowChart

```Csharp

````

```mermaid
flowchart LR
    A --> B
    B --> C
    A --> C

```

# Without Label

```mermaid
flowchart LR
   
   Trigger(New Event) --> Listner

```
# Assign a Label
```mermaid
flowchart LR
   
   Trigger(New Event) --> Listner

```

# Circle
```mermaid
flowchart LR
   
   Trigger((New Event)) --> Listner

```

# more shapes
```mermaid
flowchart LR
    Trigger((New Event)) --> Listner
    Listner --> Kafka(Kafka Events Topic)
    Kafka --> Handler[New Event Handler]
    Handler --> db[(Database)]
    Handler --> mail[/Send Notification/]

```


# decision making
```mermaid
flowchart TD
    A[Deploy to Production] --> B{Is it Friday?};
    B --Yes --> C[Do not Deploy!];
    B --No --> D[Run Deploy.sh to deploy!];
    C --> E[Enjoy your weekend!]
    D --> E[Enjoy your weekend!]
```

# With hyyperlink and Tooltip
```mermaid
flowchart LR;
    A-->B;
    B-->C;
    C-->D;
    click A callback "Tooltip for a callback"
    click B "http://www.github.com" "This is a tooltip for a link"
    click A call callback() "Tooltip for a callback"
    click B href "http://www.github.com" "This is a tooltip for a link"

    ```
