# Plan de Identificación y Preservación - Caso Almadraba

Elena, son las 10:45 y esto es lo que voy a hacer. Hasta que sepamos qué ocurrió, todo lo que hay en la oficina es evidencia potencial, así que lo primero es no perder nada y no alterar nada. A continuación explico qué hay que proteger, qué se pierde si esperamos y qué necesito pedir a otras personas. Antes de actuar confirmo por escrito con Elena qué equipos, cuentas y personas cubre la autorización que me ha firmado (L1); los dispositivos personales solo los toco con consentimiento o mandato. Las referencias L1, L2... remiten a los puntos de mi [lista de comprobación](lista-comprobacion.md).

## 1. Las fuentes de evidencia

Inventario por ubicación, con quién controla cada fuente, porque eso condiciona lo que puedo hacer con ella.

### A la vista, en la mesa de Marta

| Fuente | Qué puede aportar | Titularidad o control |
| :--- | :--- | :--- |
| Portátil Dell (encendido, bloqueado, con BitLocker) | Memoria RAM, sesiones abiertas, conexiones activas, historial de dispositivos USB conectados, ficheros y sincronización con OneDrive | Empresa |
| Dock USB-C, monitores, teclado y ratón | Qué está conectado y cómo. Valor técnico bajo | Empresa |
| Disco externo negro de 2 TB (conectado al dock) | Posible copia de proyectos | Por confirmar, no consta que sea de la empresa |
| iPhone de empresa | WhatsApp con clientes, fotos, posible copia en iCloud | Empresa |

### En manos de personas concretas

| Fuente | Qué puede aportar | Titularidad o control |
| :--- | :--- | :--- |
| Móvil personal de Marta (asoma del bolso) | Desconocido. Ella afirma que no hay nada del trabajo | Personal de Marta |
| Pendrive de Javier (en su cajón) | Marta lo usó esa semana, puede conservar rastros de copiado | De Javier |
| Sobremesa compartido de la entrada | Historial local de impresión y escaneo. Tiene abierta una sesión de Outlook de otra compañera, que no es fuente del caso | Empresa |

### Deducidas del relato

| Fuente | Qué puede aportar | Titularidad o control |
| :--- | :--- | :--- |
| Pendrive original de Marta, que "no le funcionaba" | Si no funcionaba, ¿por qué pidió otro? Su paradero es desconocido | Por confirmar |
| Equipos de Marta en casa (teletrabaja los viernes) | Posibles copias | Fuera del control de la empresa |
| Propuesta del estudio de Sevilla que el cliente enseñó a Elena (si Elena conserva copia, captura o correo) | La versión del render que circula, con su fecha y sus metadatos si existen | Cadena hotelera y Elena |
| Personas: Marta, Javier, Elena, la compañera de Outlook y el técnico de Bahía | Su testimonio, qué vieron y qué hicieron | No aplica |

### Infraestructura local, oculta

| Fuente | Qué puede aportar | Titularidad o control |
| :--- | :--- | :--- |
| Servidor de ficheros (cuartito) | Documentos de los proyectos y accesos, si hay auditoría | Empresa, gestiona Bahía |
| NAS de copias de seguridad (cuartito) | 14 copias nocturnas: el estado de los ficheros antes y después del día 14 | Empresa, gestiona Bahía |
| Impresora multifunción | Historial de trabajos y escaneos enviados al correo de quien los usa | Empresa |
| Cortafuegos y VPN | Registro de conexiones, incluidas las de los viernes en teletrabajo | Empresa, gestiona Bahía |
| Router, switches y punto de acceso Wi-Fi | Qué equipos estuvieron conectados y cuándo (asociaciones Wi-Fi, tabla DHCP), si el equipo lo registra | Empresa, gestiona Bahía |

### Nube y terceros

| Fuente | Qué puede aportar | Titularidad o control |
| :--- | :--- | :--- |
| Buzón y OneDrive de mgarcia (Microsoft 365) | Envíos, enlaces compartidos, versiones de ficheros, registros de auditoría de accesos y descargas | Empresa, gestiona Bahía |
| Portal de Microsoft | Claves de recuperación de BitLocker | Empresa |
| Copia en iCloud del iPhone de empresa, si existe | Mensajes y fotos | Por confirmar |
| Cámara domo del pasillo y grabador de conserjería | Quién entró y salió, y a qué hora, el día 14 | Administración de la comunidad |

Queda fuera del alcance contactar con Lucía Navarro o con el estudio de Sevilla. Eso, si procede, será una decisión posterior con asesoría jurídica.

## 2. La prioridad

Hoy es día 20. El día 14, cuando Marta se quedó hasta tarde, es el hecho sospechoso que conocemos, pero el render se presentó hace dos semanas y la ventana de interés empieza antes, así que pido todo lo que siga existiendo y no solo lo del día 14. Ordeno las fuentes por lo que antes se pierde, no solo por la memoria RAM: sigo el criterio de valor probable, volatilidad y esfuerzo (L16), y considero también lo que caduca con el tiempo (L17).

**Paso previo, de unos minutos:** fotografiar y anotar la escena. No cambia nada y fija el estado inicial. Después, por este orden:

1. **Registros que se sobrescriben con el tiempo:** cortafuegos y VPN, historial de la impresora, grabaciones de la cámara, registros de auditoría de Microsoft 365 y, si existen, los registros de acceso del servidor de ficheros.
   - El cortafuegos aguanta "una semana o así" y han pasado seis días, así que los del día 14 pueden desaparecer en horas.
   - El historial de la impresora se sobrescribe con el uso normal, y el sobremesa compartido lo usa todo el equipo.
   - Las cámaras suelen conservar poco tiempo y la nube tiene plazos de retención limitados. En ambos casos hay que confirmar el plazo.
2. **Copias del NAS.** Con 14 copias nocturnas, la del día 14 sobrevive unos días más, pero cada noche se descarta la más antigua, y esta noche cae aproximadamente la que ronda la fecha en que se presentó el render (hace unas dos semanas), así que la referencia del antes está al límite. Esas copias son el "antes" con el que comparar qué cambió, así que cada noche que pase se pierde una referencia.
3. **Memoria y estado del portátil encendido.** La RAM, las conexiones activas y el volumen ya descifrado se pierden si se apaga, se reinicia, se agota la batería o alguien lo manipula.
4. **Dispositivos expuestos a alteración remota:** iPhone de empresa, portátil y cuentas de Marta. Pueden ser modificados o borrados desde la nube o desde otro dispositivo.
5. **Soportes persistentes:** disco de 2 TB, pendrive de Javier, servidor de ficheros y USB desaparecido. Mientras nadie los toque sus datos no caducan. El riesgo es la manipulación, no el tiempo, así que basta con custodiarlos hoy y adquirirlos con calma. El USB desaparecido es la excepción: no puedo custodiarlo porque no sé dónde está y podría perderse u ocultarse, así que se busca hoy (L6).

**Por qué la RAM va tercera y no primera.** El RFC 3227 ordena de lo más a lo menos volátil dentro de un mismo equipo, pero aquí hay varias fuentes en varias manos. Los puntos 1 y 2 dependen de Bahía y se lanzan por teléfono, mientras yo trabajo sobre el portátil. Son acciones en paralelo, como permite el RFC 3227 §2 para equipos distintos. Dentro de cada equipo concreto sí voy paso a paso, de lo más a lo menos volátil.

## 3. Las medidas inmediatas

Cada actuación de Bahía Sistemas se hace con un parte firmado que recoja quién, qué y a qué hora, y los ficheros que entregue llevan su hash (L23, L24).

### Antes de empezar
- Fotografío la escena completa sin mover nada: puesto de Marta con ambos monitores y la pantalla bloqueada, conexiones del dock, disco, iPhone, bolso en su sitio sin abrirlo, sobremesa compartido con la sesión ajena abierta y el cuartito de informática (L4, L5).
- Me nombro custodio único de evidencias: yo fotografío, etiqueto y registro cada elemento. Abro un registro con la hora de cada acción y anoto la diferencia entre el reloj del equipo y UTC (L23, L24).
- Pido que nadie toque ni use el portátil, el disco, el iPhone ni el sobremesa compartido hasta nuevo aviso (L3).

### Medidas por fuente
- **Cortafuegos y VPN.** Llamo ahora a Bahía para que exporten el registro de conexiones completo, incluida la VPN, a un soporte externo, sin cambiar la configuración más de lo imprescindible. Les pido también que detengan la sobrescritura o amplíen la retención mientras dure el caso (L13, L17).
- **Router y punto de acceso.** Pido a Bahía que exporte qué equipos estuvieron asociados y cuándo (asociaciones Wi-Fi, tabla DHCP), si el equipo lo registra, sin reiniciarlo ni cambiar su configuración (L9, L13).
- **Impresora multifunción.** Bahía exporta el historial de trabajos. Hasta que lo haga, nadie imprime, escanea ni usa el sobremesa compartido. Son unas horas de molestia que se aceptan frente al riesgo de perder el historial (L17, L20).
- **Cámara del pasillo.** Elena escribe hoy a la administración de la comunidad pidiendo que conserven, sin borrar, las grabaciones del día 14 y de los días anteriores que aún existan, sobre todo la tarde hasta cerca de las 19 h. No pedimos verlas, solo que no se pierdan. Lo demás lo decide la administración (L11, L17).
- **NAS.** Bahía suspende la rotación de copias o separa las existentes en un soporte aparte, sin modificar su contenido (L12, L17).
- **Microsoft 365 y OneDrive.** Bahía aplica una retención de conservación sobre el buzón y el OneDrive de mgarcia, si la licencia lo permite, y exporta los registros de auditoría y el historial de versiones de los ficheros de proyecto. Es solo preservar: nadie lee el contenido del correo ahora. Una vez confirmada la retención, Elena y Bahía valoran suspender el acceso remoto de la cuenta (VPN y nube) y dejan la decisión documentada (L13, L15).
- **Portal de Microsoft.** Bahía obtiene las claves de recuperación de BitLocker de los portátiles y las guarda bajo custodia (L14).
- **Portátil Dell.** No se apaga, sigue con corriente por el dock y no se interactúa con él (L18). Después hay dos casos:
  - *Con acceso por vía formal.* Elena, como responsable del equipo de empresa, solicita por escrito a Marta las credenciales, sin darle acceso físico al equipo. Con acceso, capturo primero las conexiones activas (L19), después aíslo el equipo (L20) y por último capturo la RAM con herramientas desde un soporte protegido (L21). Capturo el estado de red antes de aislar porque las conexiones activas se pierden al cortar la red (L19, L20). El RFC 3227 §3.2 cita retirar las vías externas antes de recoger, pero su §2.1 pide empezar por lo más volátil, así que el aislamiento va justo después de esa captura.
  - *Sin acceso.* No se fuerza ni se prueban contraseñas. Se aísla, se mantiene encendido y con corriente, y se escala a un perito externo, documentando la decisión.
  - *Aislamiento.* Desconecto el cable de red del dock y pido a Bahía que bloquee el portátil en el router o punto de acceso por su dirección MAC. Así se corta el Wi-Fi sin tocar el equipo y sin dejar a la oficina sin red. Antes pregunto a Bahía si hay alguna política de borrado o bloqueo remoto que pueda dispararse, y les pido que no envíen ninguna orden remota (bloqueo, borrado, reinicio) (L20).
- **iPhone de empresa.** No lo desbloqueo ni lo apago. Lo aíslo en bolsa Faraday con batería externa o, si ya estuviera desbloqueado, en modo avión, para que no se agote. Bahía confirma que no hay una orden de borrado remoto pendiente. Se etiqueta y se registra (L7, L24).
- **iCloud del iPhone de empresa.** Averiguo con Elena y Bahía si el Apple ID es de la empresa y si hay copia en iCloud. No entro en la cuenta: solo pido que se conserve y que no se borre ni se cambie nada (L11, L15).
- **Disco externo de 2 TB.** Sigue conectado al dock hasta terminar la captura en vivo, porque desconectarlo ahora cambiaría el estado del equipo. Después se desconecta correctamente, se etiqueta y se adquiere con bloqueador de escritura. Primero confirmo de quién es (L22, L24).
- **Pendrive de Javier.** Se lo pido a Javier con su consentimiento, sin conectarlo a ningún equipo. Se entrega en bolsa etiquetada con acta de entrega firmada y se anota si lo ha usado desde entonces. Se adquiere con bloqueador de escritura (L1, L22, L24).
- **USB que falta.** No interrogo a Marta. Miro lo que está a la vista en su puesto y en las papeleras comunes, sin abrir cajones ni bolsos. La petición del pendrive original se incluye en el escrito formal de Elena. Además, una vez adquirido el portátil, el historial de dispositivos USB conectados permitirá identificar modelo y número de serie (L6).
- **Servidor de ficheros.** No se apaga. Bahía confirma si registra accesos a ficheros y preserva esos registros. La copia completa se hace después, con calma (L13, L18).
- **Sobremesa compartido.** Fotografío la sesión de Outlook ajena sin tocar nada. Después Elena pide a su titular que la cierre, porque su correo está expuesto (L4).
- **Marta.** Elena le explica con educación que hoy no podrá usar el portátil ni las cuentas de la empresa porque se están revisando los equipos, sin entrar en más detalles. Puede irse a casa y llevarse su bolso y su móvil. Anoto hora, qué dice y qué hace (L8). No se le pide ni se le revisa nada personal.
- **Testimonios.** Dejo por escrito, con fecha y hora, lo que cuentan Javier (el día 14 y el pendrive), la compañera del Outlook y el técnico de Bahía, y qué vieron y qué hicieron (L8).
- **Propuesta de Sevilla.** Pido a Elena que conserve tal cual lo que haya recibido o visto de esa propuesta (fichero, captura o correo, si existe), sin reenviarlo ni editarlo, y que anote cuándo y cómo se lo enseñó el cliente. No contacto con el estudio de Sevilla (L11, L15).

## 4. Los límites

Esto es lo que no toco, o no todavía, y qué hago en su lugar. Las referencias legales se contrastarán con asesoría jurídica antes de actuar.

- **Móvil personal de Marta.** *No lo reviso ni lo retiro.* Afectaría a su intimidad y al secreto de las comunicaciones (art. 18 CE), podría invalidar la prueba y constituir delito (art. 197 CP). *Alternativa:* pedirle por escrito, con Elena, que lo entregue voluntariamente. Si se niega, se documenta y se deja para una posible actuación judicial.
- **iPhone de empresa.** *No lo desbloqueo ni leo los WhatsApp.* Contiene conversaciones con clientes, que son terceros. *Alternativa:* aislarlo y preservarlo ahora, y examinarlo después con autorización de Elena y asesoría jurídica.
- **Contenido del correo y de OneDrive de Marta.** *Preservo pero no leo.* Acceder al contenido exige que la política de uso de medios digitales de la empresa lo permita (art. 87 LOPDGDD). *Alternativa:* retención hoy, y lectura solo con autorización de Elena y asesoría jurídica.
- **Cámara del pasillo.** *No accedo ni pido el grabador directamente.* Pertenece a la comunidad, y su acceso y tratamiento están sujetos a la normativa de videovigilancia (art. 22 LOPDGDD). *Alternativa:* petición formal de conservación a la administración y, si hace falta, requerimiento por vía judicial o policial.
- **Portátil Dell.** *No lo apago, no lo desmonto ni fuerzo el desbloqueo todavía.* Apagarlo pierde la RAM y el volumen descifrado, y forzar el acceso podría alterar la evidencia. *Alternativa:* acceso formal, o aislarlo y escalar a un perito. Con las claves de BitLocker en el portal de Microsoft, el disco se podrá adquirir después sin problema.
- **Sesión de Outlook de la compañera.** *No la exploro.* Leer su correo vulneraría su privacidad y no tiene relación con el caso. *Alternativa:* la fotografío, para dejar constancia de que el equipo estaba accesible a todos, y se cierra.
- **Pendrive de Javier.** *No lo recojo sin su consentimiento y no lo conecto a nada.* Es suyo y ha podido usarlo desde entonces. *Alternativa:* entrega voluntaria con acta, y adquisición con bloqueador de escritura.
- **Disco externo de 2 TB.** *No lo adquiero hasta saber de quién es.* Si es personal de Marta, hace falta su consentimiento o un mandato. *Alternativa:* preguntarlo por la vía formal y, hasta entonces, custodiarlo.
- **Bolso, cajones y equipos personales o domésticos de Marta.** *No los registro.* Están fuera del control de la empresa. *Alternativa:* petición escrita de entrega voluntaria.
- **Terceros externos (estudio de Sevilla, Lucía Navarro, proveedores de correo personal).** *No los contacto ni accedo a sus sistemas.* Los registros de terceros suelen requerir orden judicial. *Alternativa:* si los indicios lo justifican, denuncia o requerimiento judicial a través de asesoría jurídica.

## 5. De dónde sale cada decisión

| # | Decisión del plan | Puntos de la lista | Norma y apartado |
| :--- | :--- | :--- | :--- |
| 1 | Fotografiar la escena, designar un custodio único y abrir registro con hora | L4, L23, L24 | NIST SP 800-86 §3.1.2; RFC 3227 §2 |
| 2 | Inventariar fuentes ocultas (NAS, servidor, VPN, nube, cámara) y su titular | L9, L10, L11 | NIST SP 800-86 §3.1.1; RFC 3227 §2.1 |
| 3 | Dar prioridad a cortafuegos, impresora, cámara y auditoría de Microsoft 365 | L13, L16, L17 | NIST SP 800-86 §3.1.2, §6.2.1 y §6.2.4 |
| 4 | Parar la rotación del NAS | L12, L17 | NIST SP 800-86 §3.1.1, §2.4.3 y §3.1.2 |
| 5 | Actuar en paralelo (Bahía con logs, yo con el portátil) | L16 | RFC 3227 §2; NIST SP 800-86 §3.1.2 |
| 6 | No apagar el portátil | L18 | RFC 3227 §2.2 |
| 7 | Estado de red primero, luego aislar, luego RAM, discos al final | L19, L20, L21, L22 | RFC 3227 §2.1 y §3.2; NIST SP 800-86 §5.2.1 y §4.2.1 |
| 8 | Aislar el portátil por MAC y cable de red, sin apagar el router, y preguntar por borrado remoto | L20 | RFC 3227 §2.2; NIST SP 800-86 §3.1.3 |
| 9 | Obtener las claves de BitLocker antes de apagar o desmontar nada | L14 | RFC 3227 §2.2; NIST SP 800-86 §3.2 y §5.2.1 |
| 10 | Aislar el iPhone de empresa y mantenerlo cargado | L7 | ENFSI §8.2; NIST SP 800-86 §2.1 y §3.1.3 |
| 11 | Adquirir disco y pendrive con copia bit a bit y bloqueador de escritura | L22, L24 | RFC 3227 §2 y §2.1; NIST SP 800-86 §4.2.1 y §4.2.2 |
| 12 | Pedir el pendrive de Javier con su consentimiento y acta | L1, L6 | RFC 3227 §2.3; NIST SP 800-86 §3.1.1 |
| 13 | Buscar el USB que falta sin interrogar a Marta | L6 | ENFSI §9.2 y §11.2; NIST SP 800-86 §3.1.1 |
| 14 | No tocar el móvil personal de Marta y pedir entrega voluntaria | L1 | RFC 3227 §2.3; NIST SP 800-86 §3.1.1 |
| 15 | Pedir a la administración la conservación de la cámara, sin acceder | L1, L11 | NIST SP 800-86 §3.1.1 |
| 16 | No explorar la sesión de Outlook ajena | L1, L5 | RFC 3227 §2.3; ENFSI §9.2 |
| 17 | Preservar sin leer el buzón y el OneDrive de Marta | L1, L15 | RFC 3227 §2.3; NIST SP 800-86 §3.1.2 |
| 18 | Impedir que Marta use los equipos y anotar qué dice y qué hace | L3, L8 | ENFSI §8.2; RFC 3227 §3.2; NIST SP 800-86 §3.1.3 |
| 19 | Parte firmado y hash en cada actuación de Bahía, con cadena de custodia | L23, L24 | RFC 3227 §3.2 y §4.1; NIST SP 800-86 §3.1.2 |
| 20 | Dejar el disco de 2 TB conectado hasta terminar la captura en vivo y confirmar de quién es antes de adquirirlo | L1, L18, L22 | RFC 3227 §2.2 y §2.3; NIST SP 800-86 §3.1.1 |
| 21 | Pedir las credenciales del portátil por vía formal y, si no se obtienen, no forzar el acceso y escalar a un perito | L1, L15 | RFC 3227 §2.3 y §3.2; NIST SP 800-86 §3.1.2 |
| 22 | No apagar el servidor de ficheros y preservar sus registros de acceso | L13, L18 | RFC 3227 §2.2; NIST SP 800-86 §3.1.2 |
| 23 | Dejar por escrito lo que cuentan Javier, la compañera del Outlook y el técnico de Bahía | L8 | RFC 3227 §3.2 |
| 24 | Averiguar quién controla el iCloud del iPhone y pedir que se conserve, sin entrar en la cuenta | L11, L15 | NIST SP 800-86 §3.1.1 y §3.1.2 |
| 25 | No registrar el bolso, los cajones ni los equipos de casa de Marta, ni contactar con terceros externos | L1 | RFC 3227 §2.3; NIST SP 800-86 §3.1.1 |
| 26 | Pedir al router y al punto de acceso el registro de equipos conectados | L9, L13 | RFC 3227 §2.1; NIST SP 800-86 §3.1.1 y §6.2.1 |
| 27 | Confirmar por escrito con Elena qué cubre la autorización y tocar los dispositivos personales solo con consentimiento o mandato | L1 | RFC 3227 §2.3; NIST SP 800-86 §3.1.1 |
| 28 | No desbloquear ni leer el iPhone de empresa: aislarlo ahora y examinarlo después con autorización | L1, L7 | RFC 3227 §2.3; ENFSI §8.2; NIST SP 800-86 §3.1.1 y §3.1.3 |
| 29 | Conservar tal cual lo que Elena haya recibido de la propuesta de Sevilla, sin reenviarlo ni editarlo | L11, L15 | NIST SP 800-86 §3.1.1 y §3.1.2; RFC 3227 §3.2 |