# Modelado del proceso de negocio mediante BPMN

## 1. Objetivo del proceso

El objetivo es organizar la recepción, el análisis y la resolución de reportes de problemas relacionados con Steam. Se busca que cada reporte tenga un responsable, un estado identificable y un seguimiento hasta su cierre.

## 2. Actores del proceso

- Usuario: registra un problema y aporta la información necesaria.
- Equipo de soporte: valida los datos, clasifica el reporte y lo deriva.
- Equipo técnico: analiza el problema y propone una solución.
- Equipo de revisión: comprueba los cambios y verifica las pruebas.
- Sistema de seguimiento: registra los estados y envía notificaciones.

## 3. Flujo del proceso

1. El usuario detecta un problema y envía un reporte.
2. El sistema registra el reporte y genera un identificador.
3. El equipo de soporte verifica que la información esté completa.
4. Si faltan datos, se solicita información adicional al usuario.
5. Si los datos están completos, se clasifica el reporte y se asigna una prioridad.
6. El equipo técnico analiza el problema.
7. Si no puede reproducirse, se solicita evidencia adicional o se deja pendiente.
8. Si puede reproducirse, se prepara una corrección.
9. El equipo de revisión verifica los cambios y ejecuta las pruebas.
10. Si las pruebas fallan, la corrección vuelve al equipo técnico.
11. Si las pruebas son satisfactorias, se documenta la solución.
12. El sistema actualiza el estado y comunica el resultado al usuario.
13. El reporte se cierra.

## 4. Decisiones del proceso

- ¿La información del reporte está completa?
- ¿Se puede reproducir el problema?
- ¿Las pruebas de la solución son satisfactorias?

Estas decisiones se representan mediante compuertas exclusivas en BPMN, porque cada una permite elegir un camino según el resultado obtenido.

## 5. Organización BPMN

Se propone utilizar los siguientes pools:

- Usuario de Steam.
- Organización de soporte y desarrollo.
- Sistema de seguimiento.

Dentro del pool de soporte y desarrollo se utilizan lanes para distinguir las responsabilidades del equipo de soporte, el equipo técnico y el equipo de revisión.
