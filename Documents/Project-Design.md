# 
Authentication and Authorization
## 
Azure DevOps OAuth 2.0 Authorization Flow
 ::: mermaid
 sequenceDiagram
  participant U as User
  participant A as Your app
  participant D as Azure DevOps
  U->>A: Use your app
  A->>D: Request authorization for user
  D-->>U: Request authorization
  U->>D: Grant authorization
  D-->>A: Send authorization code
  A->>D: Get access token
  D-->>A: Send access token
  A->>D: Call REST API with access token
  D-->>A: Respond to REST API
  A-->>U: Relay REST API response
 :::
## 
User Interface
![brand.png](/.attachments/brand-ee9ffeb1-df22-48f5-89ca-d36d3b78770f.png)

