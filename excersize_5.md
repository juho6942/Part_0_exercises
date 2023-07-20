```mermaid
graph TD
  subgraph User
    U[User]
  end

  subgraph Notes App Server
    S[Server]
  end

  subgraph Browser
    B[Browser]
  end

  U -->|1. Requests SPA page| B
  B -->|2. Requests resources| S
  S -->|3. Serves SPA page| B
  B -->|4. Renders SPA| B
```
