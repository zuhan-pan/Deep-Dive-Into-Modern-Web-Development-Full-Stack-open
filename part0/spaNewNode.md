```mermaid
sequenceDiagram
participant browser
participant server

    Note right of browser: The browser re-renders the page based on input
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    server-->>browser: Status Code: 201 Created, {"message":"note created"}
    deactivate server
```
