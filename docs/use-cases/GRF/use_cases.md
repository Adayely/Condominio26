# Módulo GRF - Comunicación

## Índice

- [CU-01 Enviar Mensaje a Residentes](#cu-01-enviar-mensaje-a-residentes)
- [CU-02 Enviar Comunicado a Trabajadores](#cu-02-enviar-comunicado-a-trabajadores)
- [CU-03 Enviar Mensaje Global](#cu-03-enviar-mensaje-global)
- [CU-04 Crear Anuncio General](#cu-04-crear-anuncio-general)
- [CU-05 Modificar Anuncio General](#cu-05-modificar-anuncio-general)
- [CU-06 Eliminar Anuncio General](#cu-06-eliminar-anuncio-general)
- [CU-07 Crear Reporte de Comunicación](#cu-07-crear-reporte-de-comunicación)
- [CU-08 Consultar Historial de Mensajes](#cu-08-consultar-historial-de-mensajes)
- [CU-09 Registrar Historial de Comunicaciones](#cu-09-registrar-historial-de-comunicaciones)
- [CU-10 Notificar Mensaje Recibido](#cu-10-notificar-mensaje-recibido)

---

# CU-01 Enviar Mensaje a Residentes

## Descripción
Permite al Administrador enviar mensajes dirigidos únicamente a los residentes del condominio.

## Actor Principal
Administrador

## Precondiciones
- El Administrador debe haber iniciado sesión.
- Deben existir residentes registrados.

## Flujo Principal
1. El Administrador ingresa al módulo de comunicación.
2. Selecciona la opción de enviar mensaje a residentes.
3. Ingresa el contenido del mensaje.
4. El sistema valida la información.
5. El sistema envía el mensaje.

## Postcondiciones
- El mensaje queda registrado correctamente.

---

# CU-02 Enviar Comunicado a Trabajadores

## Descripción
Permite al Administrador enviar comunicados dirigidos a los trabajadores del condominio.

## Actor Principal
Administrador

## Precondiciones
- El Administrador debe haber iniciado sesión.
- Deben existir trabajadores registrados.

## Flujo Principal
1. El Administrador selecciona la opción de enviar comunicado.
2. Ingresa el contenido del comunicado.
3. El sistema valida los datos.
4. El sistema envía el comunicado.

## Postcondiciones
- El comunicado queda registrado correctamente.

---

# CU-03 Enviar Mensaje Global

## Descripción
Permite al Administrador enviar mensajes generales a residentes y trabajadores del condominio.

## Actor Principal
Administrador

## Precondiciones
- Deben existir usuarios registrados en el sistema.

## Flujo Principal
1. El Administrador selecciona mensaje global.
2. Ingresa el contenido del mensaje.
3. El sistema valida la información.
4. El sistema envía el mensaje a todos los usuarios.

## Postcondiciones
- El mensaje global queda registrado correctamente.

---

# CU-04 Crear Anuncio General

## Descripción
Permite al Administrador publicar anuncios generales para todo el condominio.

## Actor Principal
Administrador

## Precondiciones
- El Administrador debe haber iniciado sesión.

## Flujo Principal
1. El Administrador selecciona crear anuncio.
2. Ingresa el contenido del anuncio.
3. El sistema valida la información.
4. El sistema publica el anuncio.

## Postcondiciones
- El anuncio queda disponible para los usuarios.

---

# CU-05 Modificar Anuncio General

## Descripción
Permite modificar anuncios generales previamente publicados.

## Actor Principal
Administrador

## Precondiciones
- Debe existir un anuncio registrado.

## Flujo Principal
1. El Administrador selecciona un anuncio.
2. Modifica la información.
3. El sistema valida los cambios.
4. El sistema actualiza el anuncio.

## Postcondiciones
- El anuncio queda actualizado correctamente.

---

# CU-06 Eliminar Anuncio General

## Descripción
Permite eliminar anuncios generales registrados en el sistema.

## Actor Principal
Administrador

## Precondiciones
- Debe existir un anuncio registrado.

## Flujo Principal
1. El Administrador selecciona un anuncio.
2. Solicita la eliminación.
3. El sistema pide confirmación.
4. El Administrador confirma la acción.
5. El sistema elimina el anuncio.

## Postcondiciones
- El anuncio deja de estar disponible.

---

# CU-07 Crear Reporte de Comunicación

## Descripción
Permite generar reportes relacionados con mensajes y anuncios enviados.

## Actor Principal
Administrador

## Precondiciones
- Deben existir registros de comunicación.

## Flujo Principal
1. El Administrador selecciona generar reporte.
2. Define filtros de búsqueda.
3. El sistema consulta la información.
4. El sistema genera el reporte.

## Postcondiciones
- El reporte queda disponible para consulta.

---

# CU-08 Consultar Historial de Mensajes

## Descripción
El Administrador puede consultar el historial general de comunicaciones, mientras que los residentes y trabajadores pueden consultar únicamente los mensajes o comunicados dirigidos a ellos.

## Actor Principal
Administrador, Residente, Trabajador

## Precondiciones
- Deben existir mensajes registrados.

## Flujo Principal
1. El usuario accede al historial de mensajes.
2. Selecciona filtros de consulta.
3. El sistema muestra los mensajes registrados.

## Postcondiciones
- El historial queda visualizado correctamente.

---

# CU-09 Registrar Historial de Comunicaciones

## Descripción
Permite almacenar el historial de mensajes y anuncios realizados dentro del sistema.

## Actor Principal
Sistema

## Precondiciones
- Debe existir actividad de comunicación.

## Flujo Principal
1. El sistema detecta una acción de comunicación.
2. Guarda la información correspondiente.
3. Actualiza el historial.

## Postcondiciones
- El historial queda actualizado.

---

# CU-10 Notificar Mensaje Recibido

## Descripción
Permite al sistema notificar cuando un usuario recibe un mensaje o comunicado.

## Actor Principal
Sistema

## Precondiciones
- Debe existir un mensaje enviado.

## Flujo Principal
1. El sistema detecta un nuevo mensaje.
2. Genera una notificación.
3. Envía la notificación al destinatario.

## Postcondiciones
- El usuario recibe la notificación correctamente.