## Sistema de Gestión Documental Proyecto de la asignatura Arquitectura de Sistemas Computacionales.

Proyecto Arquitectura de Sistemas.

## Problema

 El proyecto busca desarrollar un sistema de gestión documental que permita organizar, almacenar, consultar y administrar documentos de manera centralizada y eficiente. El sistema está dirigido a organizaciones que necesitan controlar su documentación, facilitar la búsqueda de archivos y mejorar la gestión, trazabilidad y seguridad de la información.

 

## Integrantes

| Nombre | Usuario de GitHub | Rol en el equipo |
|---|---|---|
| Briyith Espinosa | IlBrithll | Integrante |
| Karen Caicedo | Kalet17 | Integrante |


## Estado del proyecto

| Hito | Estado | Tag |
|---|---|---|
| Hito 1 - Requerimientos y arquitectura | En curso | |
| Hito 2 - Infraestructura, red, datos y seguridad | Pendiente | |
| Hito 3 - Automatización, observabilidad y costos | Pendiente | |
| Hito 4 - Sustentación | Pendiente | |
| Hito 5 - Dossier final | Pendiente | |

## Estructura del repositorio

| Carpeta | Contenido |
|---|---|
| `docs/` | Documentación de arquitectura, requerimientos y decisiones |
| `docs/adr/` | Registros de decisión arquitectónica |
| `src/` | Código de la aplicación |
| `infra/` | Configuración de infraestructura |
| `tests/carga/` | Pruebas de rendimiento |
| `evidencias/` | Capturas e informes de los laboratorios |

## Hook de detección de credenciales

Después de clonar el repositorio, cada integrante debe ejecutar

git config core.hooksPath .githooks

Esta configuración es local. El hook bloquea los commits cuando
detecta posibles credenciales en los archivos preparados.
