# Plan de identificación y preservación — Almadraba Diseño

**Fecha y hora:** lunes 20 de marzo, 10:45  
**Motivo de la intervención:** posible fuga de un render confidencial presentado a un cliente.  
**Persona autorizada:** Elena Ruiz, gerente.  
**Persona sospechosa:** Marta García, cuenta `mgarcia`.

Antes de tocar nada, hay que identificar todas las posibles pruebas, decidir cuáles pueden desaparecer antes y protegerlas sin alterarlas.

## 1. Fuentes de evidencia

Estas son todas las cosas que pueden contener información sobre lo ocurrido:

### En la mesa de Marta

- **Portátil Dell de empresa**, encendido pero con la pantalla bloqueada. Puede contener archivos del render, historial de navegación, correos, WhatsApp Web, programas abiertos y datos en la memoria RAM.
- **Dock USB-C**, dos monitores, teclado y ratón. Pueden estar conectados al portátil y formar parte del mismo equipo de trabajo.
- **Disco externo negro de 2 TB.** Puede contener copias del render, archivos del proyecto o documentos relacionados con la excedencia.
- **iPhone de empresa.** Se usa para WhatsApp con clientes, por lo que puede tener mensajes, fotos, archivos enviados o recibidos y registros de uso.
- **Móvil personal de Marta.** Está en su bolso. Marta dice que no hay nada de trabajo, pero no podemos dar por hecho que sea así sin autorización y sin comprobarlo legalmente.

### En la oficina

- **Sobremesa compartido de la entrada.** Tiene una sesión abierta de Outlook web de otra compañera. Puede contener correos, archivos enviados por correo o registros de impresión y escaneo.
- **Impresora multifunción.** Escanea directamente al correo de quien la usa y guarda un historial de trabajos. Puede mostrar si Marta escaneó el render o algún documento relacionado.
- **Pendrive de Javier.** Marta lo pidió el 14 de marzo y lo devolvió al día siguiente. Puede contener archivos copiados, incluido el render.
- **Cámara del pasillo.** Es del edificio y la gestiona la administración de la comunidad. Puede mostrar quién entró o salió, a qué hora y si alguien llevó material fuera de la oficina.

### Fuera de la oficina

- **Servidor de ficheros del cuartito de informática.** Guarda los documentos de los proyectos y puede tener registros de accesos, modificaciones o descargas.
- **OneDrive.** Los documentos se sincronizan allí, por lo que puede haber versiones anteriores del render, registros de actividad y accesos desde otros dispositivos.
- **NAS de copias de seguridad.** Se hace una copia cada noche y se conservan las últimas catorce. Puede conservar versiones anteriores de los archivos.
- **Cortafuegos.** Guarda registros de conexiones, pero solo aguanta aproximadamente una semana. Puede mostrar si Marta se conectó por VPN o accedió a servicios desde fuera.
- **Portal de Microsoft / claves de BitLocker.** Puede aportar información sobre el portátil, sus accesos y las claves de recuperación.
- **Bahía Sistemas.** La consultora externa puede tener información técnica, contraseñas, configuraciones, accesos remotos y registros relacionados con los equipos.
- **Testigos.** Elena Ruiz y Javier pueden aportar información importante: quién estuvo, a qué hora, qué hizo y qué observaron.

## 2. Prioridad

El criterio principal es proteger primero lo que puede desaparecer antes. No solo la memoria RAM: también hay registros que se sobrescriben, mensajes que pueden borrarse y dispositivos que pueden desconectarse.

### Prioridad 1 — Datos que pueden perderse en minutos

1. **Portátil de Marta encendido.** Es la fuente más urgente porque está encendido. En la memoria RAM puede haber archivos abiertos, programas, conexiones y datos temporales. No debe apagarse.  
   **Lista de comprobación: “No apagar ningún sistema encendido” — RFC 3227 §2.2**

2. **Registros del cortafuegos.** Solo se conservan alrededor de una semana. Si se espera, pueden sobrescribirse y perderse las conexiones de esos días.  
   **Lista de comprobación: “Preguntar por registros remotos” — RFC 3227 §2.1, §3.2; NIST SP 800-86 §3.1.1**

3. **iPhone de empresa.** Los mensajes de WhatsApp, fotos y archivos pueden borrarse o modificarse fácilmente. También puede haber notificaciones o sesiones abiertas.  
   **Lista de comprobación: “Hacer inventario de dispositivos” — NIST SP 800-86 §3.1.1**

4. **Sesión de Outlook abierta en el sobremesa compartido.** Puede cerrarse sola, cerrarse por inactividad o modificarse. Hay que documentarla antes de que desaparezca.  
   **Lista de comprobación: “Fotografiar y documentar el estado inicial” — ENFSI §8.2**

### Prioridad 2 — Datos que pueden alterarse o desaparecer pronto

5. **Pendrive de Javier.** Puede contener archivos copiados por Marta. Hay que asegurarlo cuanto antes para que nadie lo use, lo borre o lo sobrescriba.  
   **Lista de comprobación: “Inventario de dispositivos” — NIST SP 800-86 §3.1.1**

6. **Disco externo de 2 TB.** Puede contener el render o copias de archivos. Hay que identificarlo y evitar que se conecte a otro equipo antes de analizarlo.  
   **Lista de comprobación: “Inventario de dispositivos” — NIST SP 800-86 §3.1.1**

7. **Historial de la impresora.** No se sabe cuánto tiempo conserva los trabajos. Puede demostrar si se escaneó el render y a qué correo se envió.  
   **Lista de comprobación: “Preguntar por registros remotos” — RFC 3227 §2.1, §3.2**

8. **OneDrive y servidor de ficheros.** Pueden tener registros de accesos, descargas, modificaciones y versiones anteriores. Hay que pedir que se conserven antes de que alguien borre o sincronice archivos.  
   **Lista de comprobación: “Preguntar por copias de seguridad y datos fuera del equipo” — RFC 3227 §2.1, §3.2; NIST SP 800-86 §3.1.1**

9. **NAS de copias de seguridad.** Aunque conserva catorce copias, puede sobrescribirse con nuevas copias nocturnas. Hay que pedir que se protejan las copias anteriores al incidente.  
   **Lista de comprobación: “Preguntar por copias de seguridad” — RFC 3227 §2.1, §3.2**

### Prioridad 3 — Información que puede solicitarse a terceros

10. **Cámara del pasillo.** Las grabaciones pueden borrarse automáticamente después de unos días. Hay que pedir cuanto antes a la administración del edificio que las conserve.  
    **Lista de comprobación: “Identificar sistemas remotos” — NIST SP 800-86 §3.1.1**

11. **Registros de Microsoft, OneDrive y BitLocker.** Hay que pedirlos a través de Bahía Sistemas o de los responsables correspondientes.  
    **Lista de comprobación: “Identificar sistemas remotos” — NIST SP 800-86 §3.1.1**

12. **Testimonios de Elena y Javier.** Hay que recogerlos por escrito cuanto antes, porque con el tiempo pueden olvidar detalles.  
    **Lista de comprobación: “No olvidar a las personas” — RFC 3227 §3.2**

## 3. Medidas inmediatas

### Portátil de Marta

- **No apagarlo.** Está encendido y bloqueado; apagarlo podría destruir información de la memoria.
- **No intentar adivinar la contraseña ni desbloquearlo.**
- **Fotografiar la pantalla bloqueada, el portátil, el dock, los monitores, los cables y el disco externo.**
- **Aislarlo de la red solo si se confirma que desconectarlo no va a borrar datos remotos.** Antes hay que consultar con Bahía Sistemas, porque Marta usa VPN y los archivos se sincronizan con OneDrive.
- **Si es posible y está autorizado, capturar primero la memoria RAM y los datos volátiles con herramientas forenses desde un medio externo.**  
  **Lista de comprobación: “No apagar ningún sistema encendido”, “No confiar en programas del propio equipo”, “Priorizar lo más volátil” — RFC 3227 §2.1, §2.2, §5**

### Disco externo

- **No conectarlo a ningún ordenador normal.**
- **Fotografiarlo y anotar marca, modelo, capacidad y número de serie.**
- **Guardarlo en un lugar seguro hasta poder hacer una copia forense.**  
  **Lista de comprobación: “Inventario de dispositivos”, “Minimizar cambios en el sistema” — NIST SP 800-86 §3.1.1; RFC 3227 §2, §2.2**

### iPhone de empresa

- **No desbloquearlo ni revisar WhatsApp manualmente.**
- **Fotografiar la pantalla tal como está.**
- **Activar el modo avión o aislarlo de la red, si eso no impide recuperar datos necesarios.**
- **Guardarlo en una bolsa de bloqueo de señal si se dispone de una.**
- **Pedir autorización específica antes de analizarlo.**  
  **Lista de comprobación: “Inventario de dispositivos”, “Documentar cada adquisición” — NIST SP 800-86 §3.1.1; RFC 3227 §3.1–3.2**

### Móvil personal de Marta

- **No tocarlo.** Es un dispositivo personal y Marta ha dicho que no contiene información laboral.
- **No revisarlo sin su consentimiento expreso o una autorización legal adecuada.**
- **Documentar que existe, dónde está y qué ha declarado Marta sobre él.**  
  **Lista de comprobación: “Comprobar autorización legal y alcance” — RFC 3227 §2.3–2.4; NIST SP 800-86 §3.1.1**

### Sobremesa compartido

- **Fotografiar la sesión de Outlook abierta antes de cerrarla o tocarla.**
- **No cerrar sesión ni enviar, borrar o abrir correos.**
- **Pedir a la compañera propietaria de la cuenta que no la cierre y que informe si recibe algún aviso.**
- **Si es necesario, hacer una captura o adquisición forense con autorización.**  
  **Lista de comprobación: “Fotografiar y documentar el estado inicial” — ENFSI §8.2**

### Pendrive de Javier

- **Pedir a Javier que lo entregue y que no lo conecte a ningún equipo.**
- **Fotografiarlo y guardar en una bolsa o caja etiquetada.**
- **Registrar quién lo entrega, a qué hora y en qué estado está.**  
  **Lista de comprobación: “Inventario de dispositivos”, “Documentar cada adquisición” — NIST SP 800-86 §3.1.1; RFC 3227 §3.1–3.2**

### Impresora multifunción

- **Pedir a Bahía Sistemas o a la persona responsable que no borre el historial de trabajos.**
- **Solicitar una copia o exportación del historial cuanto antes.**
- **Fotografiar las pantallas o menús donde se vea el historial.**  
  **Lista de comprobación: “Preguntar por registros remotos” — RFC 3227 §2.1, §3.2**

### Servidor de ficheros, OneDrive, NAS y cortafuegos

- **Contactar de inmediato con Bahía Sistemas.**
- **Pedir que se congelen o exporten los registros del cortafuegos antes de que se sobrescriban.**
- **Pedir que se conserven los registros de acceso al servidor de ficheros y de actividad en OneDrive.**
- **Pedir que no se sobrescriban las copias de seguridad del NAS, especialmente las anteriores al 14 de marzo.**
- **Solicitar información sobre accesos por VPN, dispositivos conectados y actividad de la cuenta `mgarcia`.**  
  **Lista de comprobación: “Preguntar por copias de seguridad, registros remotos y datos fuera del equipo” — RFC 3227 §2.1, §3.2; NIST SP 800-86 §3.1.1**

### Cámara del pasillo

- **Llamar o escribir a la administración de la comunidad.**
- **Pedir formalmente que conserven las grabaciones desde varios días antes del 14 de marzo hasta la fecha actual.**
- **Solicitar una copia de las grabaciones relevantes, especialmente las que muestren entradas y salidas de Marta o de otras personas.**  
  **Lista de comprobación: “Identificar sistemas remotos” — NIST SP 800-86 §3.1.1**

### Testigos

- **Tomar declaración escrita a Elena Ruiz y Javier.**
- **Preguntar por fechas, horas, acciones concretas y objetos implicados.**
- **No sugerir respuestas ni influir en su relato.**  
  **Lista de comprobación: “No olvidar a las personas” — RFC 3227 §3.2**

## 4. Límites

### Lo que no debemos hacer

- **No apagar el portátil de Marta.** Podría borrar información de la memoria RAM y de programas abiertos.  
  **RFC 3227 §2.2**

- **No revisar el móvil personal de Marta.** Es un dispositivo privado. Aunque Elena sospeche de ella, no tenemos derecho a registrarlo sin consentimiento o autorización legal.  
  **RFC 3227 §2.3–2.4**

- **No usar el ordenador de Marta ni abrir archivos directamente.** Abrir documentos, navegar por carpetas o usar programas del equipo puede modificar fechas de acceso y alterar pruebas.  
  **RFC 3227 §2, §2.2**

- **No cerrar la sesión de Outlook abierta en el sobremesa compartido.** Podría perderse información visible en ese momento.  
  **ENFSI §8.2**

- **No borrar, mover ni sobrescribir archivos del servidor, OneDrive o NAS.** Hay que pedir que se conserven y, si hace falta, hacer copias forenses.  
  **RFC 3227 §2.1, §3.2**

- **No acusar a Marta ni tomar decisiones basadas solo en sospechas.** La relación con Lucía, la excedencia y el hecho de quedarse tarde son indicios, no pruebas. Hay que buscar evidencia objetiva.

### Qué hacer en su lugar

- Documentar todo lo que se ve sin modificarlo.
- Fotografías, notas, hora y personas presentes.
- Aislar dispositivos solo cuando sea seguro hacerlo.
- Pedir a Bahía Sistemas que conserve registros y copias de seguridad.
- Solicitar las grabaciones de la cámara a la administración del edificio.
- Recoger declaraciones de Elena y Javier.
- Usar herramientas forenses desde medios externos y de solo lectura.
- Mantener una cadena de custodia: quién tiene cada prueba, cuándo y qué se ha hecho con ella.

## Resumen

Lo más urgente es proteger el **portátil encendido**, los **registros del cortafuegos**, el **iPhone de empresa** y la **sesión de Outlook abierta**, porque pueden perderse o modificarse rápidamente. Después hay que asegurar el **pendrive**, el **disco externo**, el **historial de la impresora**, el **servidor de ficheros**, **OneDrive** y el **NAS**.

También hay que pedir ayuda a terceros: **Bahía Sistemas** para los registros técnicos y copias de seguridad, y la **administración del edificio** para conservar las grabaciones de la cámara.

El móvil personal de Marta no debe tocarse sin autorización. La prioridad es conservar las pruebas, no demostrar de antemano que Marta es responsable.
