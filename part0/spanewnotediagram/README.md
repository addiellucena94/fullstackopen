### 0.4: SPA New Note diagram
```mermaid
sequenceDiagram;
    participant Client;
    participant Server;

    Client->>Server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa;
    Server-->>Client: application/json charset=utf-8;

    Note right of Client: The browser show de web page;
```