```mermaid
sequenceDiagram;
    participant browser
    participant server
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa

    Note right of browser: Request Payload {content: "testspa", date: "2023-02-17T11:54:38.155Z"}

    activate server
    server-->>browser: {"message":"note created"}
    deactivate server
    
    Note right of browser: The browser executes the callback function that renders the notes 
    

  ```