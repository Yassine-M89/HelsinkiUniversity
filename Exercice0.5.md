```mermaid

sequenceDiagram
    autonumber
    participant client
    participant server
    client->>server: HTTP Get "https://studies.cs.helsinki.fi/exampleapp/spa"
    server ->> client : HTML Code
    client ->> server : HTTP Get "https://studies.cs.helsinki.fi/exampleapp/main.css"
    server ->> client : main.css
    client ->> server : HTTP Get "https://studies.cs.helsinki.fi/exampleapp/spa.js"
    server ->> client : spa.js
    client ->> server : HTTP Get "https://studies.cs.helsinki.fi/exampleapp/data.json"
    server ->> client : data.json
```