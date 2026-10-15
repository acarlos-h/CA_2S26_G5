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

## 3. Diagrama de flujo
<img width="6533" height="8192" alt="Diagrama de FlujoSolución" src="https://github.com/user-attachments/assets/717124ba-92f6-427c-b78d-e8b509732416" />

## 4. Cómo interactúa el usuario con el sistema paso a paso

1. **Abrir el asistente.** Don Rony abre la aplicación y ve la pantalla principal con botones grandes.
2. **Buscar el carro.** Escribe la placa en el expediente digital. Si no existe, lo crea con la placa, el dueño y su teléfono y si ya existe, ve el historial.
3. **Registrar el servicio solicitado** por el cliente.
4. **Revisar la agenda.** El sistema enseña los carros que hay en el taller y el espacio libre que hay. Si no hay espacio, ofrece otra fecha u otra hora, si hay, registra el carro con su hora estimada de salida.
5. **Armar el presupuesto.** Tras revisar el carro, elige la mano de obra, los repuestos y el tiempo estimado, y el sistema suma el total.
6. **Enviar el presupuesto.** Presiona el botón que prepara el mensaje y don Rony lo envía al cliente.
7. **Esperar la aprobación.** Si el cliente no aprueba, se ajusta el presupuesto o se cierra el caso, si aprueba, continúa el trabajo.
8. **Controlar los repuestos.** Registra el repuesto, el proveedor, el precio y su estado: pedido, en camino o ya llegó.
9. **Realizar la reparación.** Si aparece otro daño, vuelve al paso 5 y envía un segundo presupuesto.
10. **Registrar el cobro.** Anota cuánto se cobró y si ya se pagó (sin facturación).
11. **Guardar en el expediente.** El servicio queda en el historial del carro.
12. **Guardado y respaldo.** Todo se guarda en el celular y se respalda en internet cuando hay señal.
13. **Entregar el carro** al cliente.

