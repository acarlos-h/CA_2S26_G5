# Diagrama de Flujo de la Solución Propuesta
## 1. Introducción
Este documento presenta de forma visual la solución tecnológica que el equipo decidió en la **Junta Directiva Técnica** para el taller **AutoSemec** propiedad de don **Rony Payes**. 
Se trata de la **Fase 1**: un asistente en el celular que reúne en una sola aplicación el expediente digital de cada carro, la lista de repuestos, el presupuesto con un registro de cobro y una agenda simple con control de espacio.

El diagrama muestra cómo funciona la solución de principio a fin cómo la usa don Rony, qué hace el sistema, dónde se guarda la información y cuándo puede llegar un cliente. Parte de los problemas que se encontraron en la entrevista y que respeta lo decidió en la junta

## 2. Justificación

La solución es una **aplicación móvil (asistente en el celular)**. No es un
sistema de escritorio ni una página web, porque don Rony trabaja con las manos
y ya lleva el celular consigo todo el día.

| Componente | Dónde está | Qué hace |
|---|---|---|
| **Aplicación asistente** | Celular de don Rony | Pantalla principal con botones grandes desde la que se accede a todas las funciones. |
| **Sistema local** | Celular de don Rony | Guarda lo que se escribe aunque falle la señal de internet. |
| **Respaldo en la nube** | Internet | Guarda una copia de los datos. Si se pierde el teléfono, se entra desde otro y la información sigue ahí. |
| **Mensaje al cliente** | Teléfono del cliente | Recibe el presupuesto y responde si lo aprueba. No necesita instalar nada. |

Decisiones del entorno tomadas en la junta:

- Todo vive en una sola aplicación, porque don Rony no quiere usar muchas.
- Lo escrito no se pierde aunque falle el internet.
- El botón del presupuesto prepara el mensaje, pero don Rony lo envía y los avisos automáticos quedan para la Fase 2.
  
