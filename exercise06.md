    sequenceDiagram
        participant browser
        participant server

        Note right of browser: We send a POST request to the server with the note

        browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
        activate server

        server-->>browser: {"message":"note created"}
        deactivate server