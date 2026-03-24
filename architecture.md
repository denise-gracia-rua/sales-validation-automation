# 🧩 Arquitectura del flujo

```mermaid
flowchart TD

A[Google Forms - Registro de venta] --> B[Google Sheets]
B --> C[Automatización]
C --> D[API Validación RUC]
D --> E{¿Comercio válido?}

E -->|Sí| F[Venta validada]
E -->|No| G[Venta rechazada]

F --> H[Notificación al equipo]
G --> H


5. Click en **Commit changes**

---

## 💥 Después:

Volvé a tu README y agregá esta línea debajo de “Arquitectura del flujo”:

```markdown
📌 Ver diagrama: architecture.md

## 📏 Métricas de éxito

- % de ventas validadas automáticamente
- Reducción de errores manuales
- Tiempo de validación por venta
- Impacto en reportes comerciales

## ⚠️ Riesgos considerados

- Dependencia de API externa
- Calidad de datos de entrada
- Manejo de errores en validación

## 🔐 Consideraciones

- Protección de datos sensibles
- Validaciones adicionales en inputs
