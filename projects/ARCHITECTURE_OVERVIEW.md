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
    end;
    subgraph Frontend
        direction LR
        E["Backend for Frontend (SSR/SSG)"]<--|req|F[React Frontend];
        F-->|res|E;
    end;
    Frontend-->|req|Backend;
    Backend-->|res|Frontend;
```