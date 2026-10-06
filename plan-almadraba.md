# Plan de Identificación y Preservación - Caso Almadraba

## 1. Las fuentes de evidencia
A partir del análisis de la escena y de la entrevista, se deducen fuentes a la vista, ocultas y en manos de terceros:

*   **En la mesa y entorno de Marta:** Portátil Dell (encendido y bloqueado), dock USB-C, dos monitores, teclado, ratón, disco externo de 2 TB negro y su iPhone de empresa.
*   **En posesión de Marta:** Teléfono móvil personal (asoma del bolso).
*   **En otros puestos:** Pendrive prestado de Javier (en su cajón) y ordenador de sobremesa compartido (con sesión web de Outlook de otra persona).
*   **La evidencia deductiva (lo que falta):** El pendrive original de Marta que supuestamente "no le funcionaba" el jueves 14. 
*   **Infraestructura local y red (ocultas):** Servidor de ficheros, NAS de copias de seguridad, historial de trabajos de la impresora multifunción y registros de conexión del cortafuegos.
*   **Nube y Terceros:** Portal de Microsoft (claves BitLocker), servicio OneDrive (sincronización en la nube) y la cámara domo del pasillo (grabador en conserjería).

## 2. La prioridad
El orden de preservación viene marcado por el riesgo inminente de destrucción y la volatilidad temporal, no solo por la RAM:

1.  **Registros volátiles a punto de sobrescribirse:** Cortafuegos e impresora. El cortafuegos pisa sus datos en "una semana o así"; hoy es día 20 y el incidente fue el 14, la prueba está a horas de desaparecer. El historial de la impresora puede borrarse con cualquier nuevo escaneo. Las grabaciones de la cámara de conserjería también suelen tener ciclos cortos.
2.  **Copias de seguridad en rotación:** El NAS guarda los últimos 14 días. Si el sistema sigue operando con normalidad, en unos días sobrescribirá la foto exacta de los ficheros del día 14.
3.  **Datos volátiles en memoria (RAM y conexiones):** El portátil Dell está encendido. Si se le agota la batería o se apaga, se perderá la memoria RAM (que contiene procesos, portapapeles) y el equipo se bloqueará por el cifrado BitLocker.
4.  **Aislamiento de la nube:** Dispositivos sincronizados (iPhone, portátil). Riesgo crítico de borrado remoto (wiping) o alteraciones a través de OneDrive.
5.  **Almacenamiento persistente físico:** Disco de 2 TB, pendrive de Javier, el USB perdido y el servidor de ficheros. Tienen prioridad baja porque, mientras nadie los manipule, los datos no caducan.

## 3. Las medidas inmediatas
Acciones a ejecutar de inmediato para cada fuente identificada:

*   **Cortafuegos e Impresora:** Llamar a Bahía Sistemas para que extraigan de inmediato un volcado de los logs del cortafuegos y el historial de red de la impresora, garantizando la cadena de custodia.
*   **Cámara del pasillo:** Pedir a Elena (gerente) que requiera urgentemente a conserjería la preservación (no borrado) de las grabaciones del día 14.
*   **NAS:** Solicitar a Bahía Sistemas que suspenda la política de rotación de copias o que aísle/congele el backup correspondiente a la noche del jueves 14.
*   **Portátil Dell:** **NO apagarlo**. Asegurar que recibe corriente por el dock. Aislarlo de la red (desconectar cable Ethernet o router Wi-Fi) para evitar borrados desde la nube y preparar un volcado de RAM en vivo.
*   **iPhone de empresa:** Ponerlo en modo avión (si está desbloqueado) o introducirlo en una bolsa Faraday para aislarlo de la red.
*   **Pendrive de Javier:** Recogerlo del cajón de Javier y documentar su adquisición (bolsa de evidencias).
*   **El USB que falta:** Buscarlo físicamente en la papelera o la mesa, o preguntar a Marta dónde desechó el pendrive averiado para intentar recuperarlo.
*   **Portal Microsoft:** Pedir a Bahía Sistemas que exporte y facilite el acceso a las claves de recuperación de BitLocker.

## 4. Los límites
Elementos sobre los que no podemos o no debemos actuar directamente, y sus alternativas:

*   **Móvil personal de Marta:** *No se puede tocar* porque vulneraría su derecho fundamental a la intimidad y secreto de comunicaciones; invalidaría la prueba y es delito. *Alternativa:* Requerirle amistosamente y por escrito que lo entregue de forma voluntaria. Si se niega, se documenta para una posible solicitud judicial.
*   **Cámara de vigilancia:** *No se puede tocar* porque pertenece a un tercero (la comunidad), accediendo cometeríamos una infracción de protección de datos. *Alternativa:* Trámite formal a través de la gerencia hacia la administración del edificio.
*   **Portátil (extracción de disco duro):** *No se puede apagar ni desmontar todavía.* Al tener BitLocker, un apagado abrupto forzará el bloqueo del disco y perderemos la clave en memoria. *Alternativa:* Hacer la captura de RAM en vivo primero, conseguir la clave en el portal de Microsoft y luego apagar ordenadamente.
*   **Sesión de Outlook de la compañera:** *No se debe explorar.* Aunque la sesión esté abierta en el equipo compartido, inspeccionar correos ajenos al caso vulnera la privacidad de esa empleada. *Alternativa:* Documentar fotográficamente que la sesión estaba abierta y el equipo accesible a todos, pero no interactuar con el correo.

## 5. De dónde sale cada decisión
Justificación apoyada en los puntos de la lista de comprobación y las normativas forenses:

*   **Puntos 5, 6 y 9:** Justifican la identificación exhaustiva de fuentes visibles e invisibles (incluyendo la deducción del USB perdido y la consulta por servidores/NAS/cámaras). *(Norma ENFSI / NIST SP 800-86)*
*   **Puntos 12 y 15:** Justifican la prioridad crítica dada al cortafuegos, la impresora, el NAS y las cámaras, priorizando aquellos registros volátiles y copias que caducan o se sobrescriben. *(Norma NIST SP 800-86)*
*   **Puntos 16, 19 y 20:** Justifican el límite de no apagar el portátil y la decisión de mantenerlo encendido para realizar primero una recolección de memoria (RAM) por el orden estricto de volatilidad. *(Norma RFC 3227)*
*   **Puntos 7 y 17:** Justifican las medidas inmediatas de aislar el iPhone y el portátil de la red para evitar la alteración remota de evidencias sin alterar el sistema local. *(Norma ENFSI / RFC 3227)*
*   **Puntos 13:** Justifica la solicitud inmediata de las claves de BitLocker a Bahía Sistemas antes de proceder con el portátil. *(Norma ENFSI)*