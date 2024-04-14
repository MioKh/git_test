a test for fullstackopen

```mermaid
sequenceDiagram
    participant User
    participant Browser
    participant Server

    User->>Browser: Enters URL https://studies.cs.helsinki.fi/exampleapp/spa
    Browser->>Server: GET /spa
    activate Server
    Server-->>Browser: SPA HTML document
    Browser->>Server: JavaScript execution
    Server-->>Browser: Execute SPA JavaScript
    Browser->>Server: Fetch data.json
    Server-->>Browser: JSON data
    Browser-->>Server: Render notes from JSON data
```

testing other graphs 

```mermaid

graph LR;
    A[Head] --> B[Node 1]
    B --> C[Node 2]
    C --> D[Node 3]
    D --> E[Node 4]
    E --> F[Null]

```

```mermaid
graph TD;
    A[Root] --> B[Left Child]
    A --> C[Right Child]
    B --> D[Left Grandchild]
    B --> E[Right Grandchild]
    C --> F[Left Grandchild]
    C --> G[Right Grandchild]
```

```mermaid
graph TD;
    A[Sorted Array] --> B(Start)
    B --> C{Find middle element}
    C -->|Equal| D(Return middle index)
    C -->|Less| E(Search left half)
    C -->|Greater| F(Search right half)
    E -->|Empty subarray| G(Return not found)
    F -->|Empty subarray| H(Return not found)
    E --> C
    F --> C

    %% Add titles to each node
    style A fill:#EAEAEA,stroke:#333,stroke-width:2px;
    style B fill:#EAEAEA,stroke:#333,stroke-width:2px;
    style C fill:#EAEAEA,stroke:#333,stroke-width:2px;
    style D fill:#EAEAEA,stroke:#333,stroke-width:2px;
    style E fill:#EAEAEA,stroke:#333,stroke-width:2px;
    style F fill:#EAEAEA,stroke:#333,stroke-width:2px;
    style G fill:#EAEAEA,stroke:#333,stroke-width:2px;
    style H fill:#EAEAEA,stroke:#333,stroke-width:2px;

    ```


