### 0.4: New note diagram
```mermaid
sequenceDiagram;
    participant Client;
    participant Server;

    Client->>Server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note;
    Server-->>Client: text/html charset=UTF-8;

    Client->>Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes;
    Server-->>Client: text/html charset=UTF-8;

    Client->>Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css;
    Server-->>Client: text/css charset=UTF-8;

    Client->>Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js;
    Server-->>Client: application/javascript charset=UTF-8;

    Client->>Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json;
    Server-->>Client: application/json charset=UTF-8;

    Note right of Client: The browser show de web page;
```