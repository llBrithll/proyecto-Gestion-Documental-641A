# Requerimientos no funcionales

| # | Atributo | Métrica | Umbral | Condición de carga | Verificación | Consecuencia si no se cumple |
|---|---|---|---|---|---|---|
| 1 | Rendimiento | p95 de latencia | Menor a 400 ms | 200 usuarios concurrentes | Prueba de carga | Los usuarios pueden percibir lentitud y abandonar el proceso de reserva |
| 2 | Disponibilidad | Porcentaje de disponibilidad mensual | Mayor o igual al 99.5% | Operación normal del sistema | Monitoreo de disponibilidad | Los pacientes no podrían consultar o gestionar sus citas |
| 3 | Seguridad | Intentos fallidos permitidos | Máximo 5 intentos consecutivos | Inicio de sesión de usuarios | Prueba funcional de autenticación | Puede aumentar el riesgo de accesos no autorizados |

## Escenarios completos

### Escenario 1 - Rendimiento

- Fuente: Paciente o personal administrativo.
- Estímulo: El usuario consulta las citas disponibles o solicita agendar una cita.
- Artefacto: Sistema de gestión de citas médicas.
- Entorno: 200 usuarios utilizando el sistema de forma concurrente.
- Respuesta: El sistema procesa la solicitud y muestra la información solicitada.
- Medida: El 95% de las solicitudes debe responder en menos de 400 ms.

### Escenario 2 - Disponibilidad

- Fuente: Paciente o personal administrativo.
- Estímulo: El usuario intenta ingresar al sistema para consultar o administrar citas.
- Artefacto: Sistema de gestión de citas médicas.
- Entorno: Operación normal.
- Respuesta: El sistema debe permanecer disponible para atender las solicitudes.
- Medida: Disponibilidad mensual igual o superior al 99.5%.

### Escenario 3 - Seguridad

- Fuente: Usuario del sistema.
- Estímulo: Se realizan varios intentos consecutivos de inicio de sesión con una contraseña incorrecta.
- Artefacto: Módulo de autenticación.
- Entorno: Operación normal.
- Respuesta: El sistema limita los intentos de acceso para proteger la cuenta.
- Medida: Máximo 5 intentos fallidos consecutivos antes de aplicar una medida de protección.