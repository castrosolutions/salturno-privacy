---
title: Política de privacidad de Salturno
description: Cómo Salturno trata tus datos.
---

# Política de privacidad de Salturno

**Última actualización:** 29 de mayo de 2026

Esta política describe cómo la aplicación **Salturno** (en adelante, "la
app") trata los datos personales que se generan al usarla. La app está
pensada para que un único profesional lleve **su propio cuadrante de
turnos** en su iPhone.

Para conocer los proveedores concretos que intervienen en cada parte del
servicio, consulta la página de [Subprocesadores](subprocesadores.html).
Esa lista se mantiene actualizada con independencia de esta política.

## 1. Responsable del tratamiento

- **Responsable:** Juan Pablo Castro Hurtado, persona física.
- **Contacto:** [juanpablo@castrosolutions.dev](mailto:juanpablo@castrosolutions.dev)
- **Naturaleza del proyecto:** uso personal, no comercial. La app se
  distribuye de forma gratuita y sin publicidad.

Por la naturaleza personal y no comercial del proyecto, no se ha
designado Delegado de Protección de Datos conforme al Art. 37 RGPD.

## 2. Principio general: la app es *local-first*

El dispositivo (tu iPhone) **es la fuente de verdad** de tus datos. La app
no tiene cuenta, no tiene login y no mantiene una copia central de tus
turnos en ningún servidor del responsable.

Tus turnos viven:

1. En el almacenamiento local de la app.
2. Replicados en **tu iCloud privado**, gestionado por Apple. El
   responsable de la app no tiene acceso a esa base de datos; es tuya y
   solo tú puedes verla desde tus dispositivos.

## 3. Dos formas de usar la app, dos niveles de tratamiento

La cantidad de datos que la app trata depende de cómo la uses.

### 3.1 Uso básico (introducción manual de turnos)

Si te limitas a usar la app como calendario y editas los turnos a mano:

- **Ningún dato personal sale hacia los servidores del responsable.**
- Tus turnos quedan en el dispositivo y, si tienes iCloud activado, se
  replican en tu iCloud privado (servicio gestionado por Apple, no por el
  responsable).

### 3.2 Importación por foto (opcional)

Esta función es **opcional**. La app solicita los permisos estándar de
iOS para **cámara** y/o **biblioteca de fotos** únicamente cuando
activas la importación, y muestra un aviso de consentimiento informando
de que la foto saldrá del dispositivo. Si deniegas los permisos o no
aceptas el aviso, la app sigue funcionando con normalidad como
calendario local; solo se inhabilita la importación por foto.

Cuando decides usar la función "Importar cuadrante" y tomas o eliges una
foto del cuadrante mensual, esa foto **viaja temporalmente fuera del
dispositivo**, junto con **tu nombre tal como lo has indicado en la
app**, para que un servicio de reconocimiento de imágenes basado en
**inteligencia artificial generativa** identifique los turnos que te
corresponden dentro del cuadrante.

En este modo:

- La foto se **procesa temporalmente en servidores ubicados en la Unión
  Europea**.
- Como parte de ese procesamiento se utiliza un **servicio de
  inteligencia artificial generativa de un tercero**, que puede operar
  fuera del Espacio Económico Europeo (ver §6). El proveedor concreto
  está identificado en la página de
  [Subprocesadores](subprocesadores.html).
- El resultado (un listado estructurado de turnos y nombres tal como
  aparecen en el cuadrante) se entrega a tu dispositivo, que lo integra
  en tu calendario.

Tras el procesamiento se aplican borrados automáticos en los plazos
máximos publicados en §8.

El reconocimiento de la imagen es un proceso **automatizado**, pero su
**resultado es revisable por ti antes de integrarse en tu calendario**:
la app no añade turnos a ciegas. Este procesamiento **no toma decisiones
que produzcan efectos jurídicos** sobre ti ni que te afecten
significativamente de modo similar, en el sentido del Art. 22 RGPD.

Los datos enviados al servicio de reconocimiento de imágenes **no se
utilizan para entrenar modelos de inteligencia artificial**, conforme a
las condiciones de uso contratadas con el proveedor. **Tampoco se vende
información personal a terceros**, ni con esa finalidad ni con ninguna
otra.

### 3.3 Identidad técnica anónima de la instalación

Para evitar el uso abusivo del servicio de importación, la app genera un
**identificador técnico anónimo** asociado a tu instalación, utilizando
**los mecanismos de validación de instalación que proporciona el sistema
operativo del dispositivo**, apoyados en sus capacidades de seguridad.

**Este identificador no es publicitario ni de seguimiento.** No contiene
datos personales tuyos: no incluye nombre, Apple ID, IDFA, IDFV, número
de teléfono, ubicación ni ningún otro dato que permita asociarlo a una
persona concreta o cruzarlo con otras apps. Se conserva mientras la app
permanezca instalada y se elimina al desinstalarla.

### 3.4 Cómo se relacionan estos datos en los sistemas del responsable

La app no tiene cuenta ni identifica al usuario de forma persistente. Por
eso es importante precisar cómo conviven entre sí los datos descritos en
§3.2 y §3.3 dentro de la infraestructura del responsable:

- Cada importación de cuadrante por foto se identifica con un
  **identificador efímero de petición** (un UUID generado en el momento).
  La foto, tu nombre tal como lo tecleas en la app y el resultado del
  reconocimiento se guardan asociados únicamente a ese identificador
  efímero, que caduca con los plazos publicados en §8 (24 horas la foto;
  72 horas el nombre y el resultado).
- El **identificador técnico anónimo de la instalación** (§3.3) se
  almacena por separado, junto con el contador anti-abuso. El responsable
  **no mantiene en ningún momento una tabla, fichero ni estructura
  interna que asocie tu nombre, la foto o el resultado del reconocimiento
  con ese identificador técnico ni con ningún otro identificador del
  usuario**.
- Una vez expirados los plazos de §8, no queda en la infraestructura del
  responsable ningún rastro asociable a tu persona. El identificador
  técnico anónimo sobrevive hasta que desinstalas la app, pero por sí
  solo no permite saber quién eres ni recuperar tus importaciones
  pasadas.

En la terminología de las plataformas de distribución (por ejemplo, las
etiquetas de privacidad de la App Store), estos datos figuran como **no
vinculados a tu identidad**: el responsable no mantiene una identidad
persistente a la que asociarlos.

### 3.5 Datos que la app no recoge

Más allá de lo descrito en §3.2, §3.3 y §3.4, la app **no** recoge en
ningún caso:

- Cuenta de usuario o credenciales (no hay registro ni inicio de
  sesión: tu nombre solo se utiliza, cuando activas la importación por
  foto, para localizar tus turnos dentro del cuadrante).
- Ubicación.
- Contactos.
- Datos de uso, analítica o telemetría comercial.
- Identificadores publicitarios.

La app **no realiza ningún tipo de seguimiento** entre apps ni sitios
web de terceros, y no presenta avisos del sistema relacionados con
seguimiento publicitario. La información publicada en la ficha de la
app en la tienda de aplicaciones complementa esta política.

## 4. Datos de terceros (compañeros de trabajo) que aparecen en el cuadrante

El cuadrante mensual del centro de trabajo contiene **nombres y turnos
de otras personas** además de los tuyos. Cuando subes la foto para
procesarla, esos datos viajan junto al resto de la imagen y siguen los
mismos plazos y garantías descritos en esta política.

**Cómo se tratan estos datos:**

- Cuando usas el reconocimiento por foto, los turnos de tus compañeros
  **también quedan almacenados localmente en tu dispositivo** (y, si
  tienes iCloud activado, en tu iCloud privado), porque forman parte del
  cuadrante reconocido. La app necesita esa información para representar
  fielmente el cuadrante que tu empleador te ha entregado.
- La base legal de este tratamiento, por la parte que afecta a los datos
  de terceros, es el **interés legítimo del usuario** (Art. 6.1.f RGPD)
  en organizar su propio trabajo a partir del cuadrante que su empleador
  le proporciona. La app no comparte esos datos con nadie ajeno al
  propio usuario.
- En la infraestructura del responsable, los datos de terceros son
  **accesorios y transitorios**: solo existen el tiempo estrictamente
  necesario para el procesamiento de la imagen, dentro de los plazos
  máximos publicados en §8.
- **Tú, como usuario, eres responsable de no compartir externamente la
  foto** del cuadrante más allá del flujo de la app.

Si eres compañero o compañera de una persona que usa Salturno y quieres
ejercer tus derechos sobre tus datos, contacta con
[juanpablo@castrosolutions.dev](mailto:juanpablo@castrosolutions.dev).

## 5. Categorías de proveedores que intervienen

El servicio se apoya en proveedores externos para infraestructura,
sincronización y procesamiento de imágenes. La lista nominal y vigente de
estos proveedores está publicada en la página de
[Subprocesadores](subprocesadores.html), con indicación de la función que
desempeña cada uno y su ubicación.

Las **categorías** de proveedores que intervienen son:

- **Plataforma del dispositivo y servicios asociados** (proveedor del
  sistema operativo iOS): para la sincronización privada con tu iCloud,
  notificaciones y validación técnica de la instalación.
- **Infraestructura cloud en la Unión Europea**: para alojar de forma
  temporal la foto durante la importación y el resultado del
  reconocimiento.
- **Servicio de reconocimiento de imágenes mediante inteligencia
  artificial**: para extraer la información estructurada del cuadrante.

El responsable puede actualizar los proveedores concretos manteniendo
**garantías equivalentes** a las descritas aquí. Cualquier cambio
sustancial se reflejará en la página de Subprocesadores y se notificará
en esta política.

Ninguno de estos proveedores utiliza tus datos para **entrenar modelos
de inteligencia artificial** ni los recibe con esa finalidad. Tampoco se
**vende información personal** a estos proveedores ni a terceros.

## 6. Transferencias internacionales

El servicio de reconocimiento de imágenes mencionado en §3.2 puede operar
**fuera del Espacio Económico Europeo**. Cuando así sea, la transferencia
se ampara en los mecanismos previstos por el RGPD para transferencias a
terceros países, en particular las **cláusulas contractuales tipo**
aprobadas por la Comisión Europea.

El resto del tratamiento — almacenamiento temporal de la foto, buzón del
resultado e identificador técnico de la instalación — se realiza dentro
de la **Unión Europea**.

## 7. Base legal del tratamiento

- **Consentimiento del interesado** (art. 6.1.a RGPD), prestado de forma
  contextual cuando activas la función de importación por foto.
- **Ejecución del servicio** solicitado por el usuario (art. 6.1.b
  RGPD): la app procesa la foto porque tú activas la importación.
- **Interés legítimo del usuario** (art. 6.1.f RGPD), aplicado en dos
  supuestos:
  - **Datos de compañeros que aparecen en el cuadrante reconocido**
    (§4): el interés legítimo del usuario en organizar su propio
    trabajo a partir del cuadrante que su empleador le proporciona
    ampara el tratamiento accesorio y transitorio de esos datos.
  - **Identificador técnico anónimo de la instalación**: se utiliza
    únicamente para impedir el uso fraudulento del servicio.

## 8. Plazos máximos de conservación

Estos plazos son **máximos**: en la práctica los datos pueden borrarse
antes.

| Dato | Plazo máximo |
|---|---|
| Datos en tu dispositivo y/o en tu iCloud privado | Bajo tu control: hasta que los borres o desinstales la app |
| Foto del cuadrante en la infraestructura del responsable | Hasta 24 horas tras la importación |
| Resultado del reconocimiento (turnos extraídos) y tu nombre asociado a la petición | Hasta 72 horas tras su procesamiento |
| Identificador técnico anónimo de la instalación | Hasta que desinstales la app |
| Registros técnicos del servicio sin contenido personal | Según el proveedor de infraestructura |

## 9. Tus derechos

De acuerdo con el RGPD y la LOPDGDD, tienes derecho a:

- **Acceso** a tus datos personales.
- **Rectificación** de datos inexactos.
- **Supresión** ("derecho al olvido"). Para los datos que viven en tu
  dispositivo y en tu iCloud, basta con borrar el contenido en la app o
  desinstalarla; los backups de iCloud se gestionan desde
  *Ajustes → iCloud → Administrar almacenamiento*. Para los datos
  residuales que pudieran quedar en sistemas intermedios, escribe al
  contacto indicado en §1 y se procederá al borrado antes de su
  expiración automática.
- **Oposición** al tratamiento basado en interés legítimo.
- **Portabilidad** de los datos que mantienes en la app, cuando
  técnicamente sea posible.
- **Presentar una reclamación** ante la **Agencia Española de Protección
  de Datos (AEPD)**: [https://www.aepd.es](https://www.aepd.es).

Para ejercer cualquiera de estos derechos, escribe a
[juanpablo@castrosolutions.dev](mailto:juanpablo@castrosolutions.dev). Se
responderá en un plazo máximo de un mes desde la recepción de la
solicitud.

## 10. Seguridad

- Las comunicaciones entre la app y los servicios del responsable se
  realizan exclusivamente sobre **HTTPS/TLS**.
- Las peticiones al servicio de importación incluyen **mecanismos de
  autenticación que aprovechan las capacidades de seguridad del
  dispositivo**, para impedir suplantación de instalaciones de la app.
- Los secretos del backend se almacenan cifrados.
- La foto durante la importación está cifrada en reposo y solo accesible
  por los componentes estrictamente necesarios para el procesamiento.

Ningún sistema es perfectamente seguro. Si detectas una vulnerabilidad,
escribe al contacto de §1.

**Notificación de brechas.** Si se produjera una brecha de seguridad de
los datos personales, el responsable la notificará a la **Agencia
Española de Protección de Datos (AEPD)** en un plazo máximo de **72
horas** desde que tenga constancia de ella, conforme al Art. 33 RGPD.
Cuando la brecha entrañe un **alto riesgo para los derechos y libertades**
de las personas afectadas, se les comunicará también a ellas sin dilación
indebida, conforme al Art. 34 RGPD.

## 11. Menores

La app no está dirigida a menores de 14 años. No se recoge
intencionadamente información de menores. Si detectas que un menor está
usando la app sin consentimiento parental, contacta al responsable.

## 12. Cambios en esta política

Cualquier cambio sustancial se reflejará actualizando la fecha al inicio
del documento. El historial completo de cambios es público en el
repositorio donde está publicada esta política.

La lista de proveedores concretos puede actualizarse con mayor frecuencia
sin que ello implique un cambio en la presente política, siempre que se
mantengan garantías equivalentes. Esa lista vive en la página de
[Subprocesadores](subprocesadores.html).

## 13. Continuidad y cese del servicio

Si el servicio operado por el responsable dejara de estar disponible:

- **Los datos en tu dispositivo y en tu iCloud privado permanecen
  intactos** mientras no desinstales la app o los borres manualmente.
  La app puede seguir funcionando localmente como calendario; solo se
  vería afectada la importación por foto, que depende de la
  infraestructura del responsable.
- En la infraestructura del responsable **no se almacena información de
  forma persistente**: los datos relacionados con cada importación se
  eliminan automáticamente tras su procesamiento.
- Cualquier dato pendiente de procesar **se eliminará igualmente al
  cesar el servicio**.

## 14. Resumen de datos tratados

A modo de visión de conjunto, esta sección recoge por categorías los
datos que trata la app, indicando si se recogen, si están vinculados a
tu identidad y si se utilizan para algún tipo de seguimiento. El criterio
para la columna *Vinculado a tu identidad* es el descrito en §3.4: si el
responsable mantiene o no, en sus sistemas, una asociación persistente
entre el dato y un identificador del usuario.

| Dato | Recogido por la app | Vinculado a tu identidad | Usado para seguimiento |
|---|---|---|---|
| Tu nombre (al usar importación por foto, §3.2) | Sí, durante el procesamiento (hasta 72 horas) | No (sin cuenta de usuario; sin asociación persistente — §3.4) | No |
| Foto del cuadrante (§3.2) | Solo si activas la importación por foto (hasta 24 horas) | No (sin asociación persistente — §3.4) | No |
| Resultado del reconocimiento (turnos extraídos, §3.2) | Sí, durante el procesamiento (hasta 72 horas) | No (sin asociación persistente — §3.4) | No |
| Turnos, notas y otro contenido en tu dispositivo y en tu iCloud privado | Sí, bajo tu control exclusivo | No accesible para el responsable | No |
| Identificador técnico anónimo de la instalación (§3.3) | Sí, únicamente para anti-abuso | No | No |
| Contactos, ubicación, identificadores publicitarios, datos de uso o analítica, diagnóstico, historial de navegación o búsqueda, compras, datos financieros, datos de salud | **No** | — | — |

La app **no realiza seguimiento** entre apps ni sitios web de terceros y
no presenta avisos del sistema relacionados con seguimiento publicitario.
En caso de discrepancia entre esta sección y el cuerpo de la política,
prevalece el cuerpo de la política.

