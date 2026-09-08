# Requerimientos no funcionales

| # | Atributo | Métrica | Umbral | Condición de carga | Verificación | Consecuencia si no se cumple |
|---|---|---|---|---|---|---|
| 1 | Rendimiento | p95 de latencia | Menor a 400 ms | 200 usuarios concurrentes | Prueba de carga | Los usuarios pueden percibir lentitud y abandonar el proceso de reserva |
| 2 | Disponibilidad | Porcentaje de disponibilidad mensual | Mayor o igual al 99.5% | Operación normal del sistema | Monitoreo de disponibilidad | Los pacientes no podrían consultar o gestionar sus citas |
| 3 | Seguridad | Intentos fallidos permitidos | Máximo 5 intentos consecutivos | Inicio de sesión de usuarios | Prueba funcional de autenticación | Puede aumentar el riesgo de accesos no autorizados |

## Escenarios completos

### Escenario 1 - Rendimiento

- Fuente: Usuario o personal administrativo.
- Estímulo: El usuario realiza una búsqueda, consulta o descarga de un documento almacenado en el sistema.
- Artefacto: Sistema de Gestión Documental.
- Entorno: Hasta 200 usuarios utilizando el sistema de manera concurrente.
- Respuesta: El sistema procesa la solicitud y muestra los documentos o la información solicitada.
- Medida: El 95% de las consultas debe responder en menos de 400 ms.

### Escenario 2 - Disponibilidad

- Fuente: Usuario o personal administrativo.
- Estímulo: El usuario intenta ingresar al sistema para consultar, cargar, descargar o administrar documentos.
- Artefacto: Sistema de Gestión Documental.
- Entorno: Operación normal del sistema.
- Respuesta: El sistema debe permanecer disponible para permitir el acceso y gestión de los documentos.
- Medida: Disponibilidad mensual igual o superior al 99.5%.