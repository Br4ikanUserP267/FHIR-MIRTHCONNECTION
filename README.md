# Grupo 2 - Documentos clínicos con FHIR Composition

## Integración con HAPI FHIR, Postman y Mirth Connect

### Integrantes
- **Braikan Piña**
- **Freydér Pérez**

---

## Pasos realizados

### 1. Crear un recurso **Composition**
Se construyó un recurso `Composition` en formato FHIR, el cual representa un **documento clínico estructurado**.  

#### Ejemplo:
```json
{
  "resourceType": "Composition",
  "status": "final",
  "type": {
    "coding": [
      {
        "code": "34133-9"
      }
    ]
  },
  "subject": {
    "reference": "Patient/1"
  }
}
