# 🧩 Arquitectura del flujo

```mermaid
flowchart TD
    A[Registro de venta - Google Forms] --> B[Google Sheets]
    B --> C[Automatización]
    C --> D[API Validación RUC]
    D --> E{¿Comercio válido?}
    E -->|Sí| F[Venta validada]
    E -->|No| G[Venta rechazada]
    F --> H[Notificación]
    G --> H
 ```
---
