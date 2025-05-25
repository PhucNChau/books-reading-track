# Notes for Developing a Full-Stack Project
[Back](../README.md)

## Overview
Architecture for developing a full-stack project.

```mermaid
flowchart LR;
    A@{ shape: cyl, label: "Database" }-->B[Data Layer];
    subgraph Backend
        B-->C[Service Layer];
        C-->D[Route Layer];
    end
    subgraph Frontend
        direction LR
        E["Backend for Frontend (SSR/SSG)"]<-->|req/res|F[React Frontend];
    end
    Backend<-->|res/req|Frontend;
```
Fig 3.1 - A modern full-stack architecture, with a single backend service and a frontend with server-side rendering (SSR) and static-site generation (SSG) - `[Modern Full-Stack React Projects by Daniel Bugl]`