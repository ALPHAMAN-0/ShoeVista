# ShoeVista
ShoeVista 👟 ShoeVista is a full-stack e-commerce web application for browsing and shopping footwear online, built on the MERN stack. It pairs a fast React + Vite frontend with a Node.js/Express REST API and a MongoDB database to deliver a smooth, modern shopping experience.

## Architecture / How it Works

```mermaid
flowchart TD
  ClientContext["Client-Context"]
  ClientApp["Client-App"]
  ClientPages["Client-Pages"]
  ClientComponents["Client-Components"]
  ServerEntry["Server-Entry"]
  ServerRoutes["Server-Routes"]
  ServerControllers["Server-Controllers"]
  ServerModels["Server-Models"]
  MongoDB["MongoDB"]

  ClientContext --> ClientApp
  ClientApp --> ClientPages
  ClientApp --> ClientComponents
  ClientApp --> ServerEntry
  ServerEntry --> ServerRoutes
  ServerRoutes --> ServerControllers
  ServerControllers --> ServerModels
  ServerEntry --> MongoDB
  ServerModels --> MongoDB
```

