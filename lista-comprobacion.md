# Lista de Comprobación Forense

## 1. Al llegar
- [ ] **1.** Preparar herramientas, software validado y material de embalaje antes de intervenir. *(ENFSI §9.1)*
- [ ] **2.** Asegurar el perímetro físico y restringir el acceso a la zona para evitar manipulación de terceros. *(ENFSI §8.2)*
- [ ] **3.** Fotografiar y documentar el estado inicial de la escena completa (pantallas, cables, entorno) antes de mover nada. *(ENFSI §8.2)*
- [ ] **4.** Identificar visualmente el estado de los ordenadores (encendidos, apagados, bloqueados) sin interactuar con ellos. *(RFC 3227 §3.1)*
- [ ] **5.** Localizar periféricos y dispositivos a la vista: móviles, discos externos, memorias USB, impresoras. *(ENFSI §9.2)*
- [ ] **6.** Buscar evidencias físicas no digitales asociadas (ej. post-its con contraseñas, agendas, manuales, cables). *(ENFSI §9.2)*
- [ ] **7.** Aislar de la red los dispositivos móviles localizados (bolsa Faraday o modo avión si es visible) para evitar borrados remotos. *(ENFSI §8.2)*

## 2. Antes de tocar nada
- [ ] **8.** Trazar visualmente la topología de la red física (routers, switches, cableado) en la oficina. *(NIST SP 800-86 §3.1.1)*
- [ ] **9.** Identificar la existencia de infraestructura local no visible (NAS, servidores de ficheros, servidor DHCP/DNS). *(NIST SP 800-86 §3.1.1)*
- [ ] **10.** Entrevistar al personal TI/Gerencia sobre servicios externos: almacenamiento en la nube, correo web, VPNs. *(NIST SP 800-86 §3.1.1)*
- [ ] **11.** Preguntar por las políticas de copias de seguridad (backups) para saber qué datos históricos existen y si rotan. *(NIST SP 800-86 §3.1.1)*
- [ ] **12.** Identificar sistemas que generen registros (logs) que se sobrescriban rápidamente (ej. cortafuegos, cámaras, impresoras). *(NIST SP 800-86 §3.1.1)*
- [ ] **13.** Verificar, consultando con responsables, si los equipos utilizan algún tipo de cifrado (BitLocker, FileVault) y dónde están las claves. *(ENFSI §9.2)*

## 3. Al decidir qué se adquiere y en qué orden
- [ ] **14.** Evaluar el valor de cada evidencia, el esfuerzo necesario para adquirirla y el riesgo de pérdida para el caso. *(NIST SP 800-86 §3.1)*
- [ ] **15.** Establecer prioridad absoluta de preservación a los registros volátiles que estén a punto de sobrescribirse o caducar (ej. cortafuegos). *(NIST SP 800-86 §3.1.1)*
- [ ] **16.** Establecer el orden de adquisición del equipo informático basándose estrictamente en el orden de volatilidad. *(RFC 3227 §2.1)*
- [ ] **17.** Asegurar que los programas de adquisición se ejecuten minimizando la alteración del sistema original (evitar instalar nada). *(RFC 3227 §2.2)*
- [ ] **18.** Iniciar un registro (log) detallado de cada comando ejecutado y cada decisión tomada durante la adquisición. *(RFC 3227 §3.2)*
- [ ] **19.** Adquirir primero la información de red del equipo (caché ARP, tablas de enrutamiento, conexiones activas). *(RFC 3227 §2.1)*
- [ ] **20.** Adquirir seguidamente el contenido íntegro de la memoria principal (RAM) y los procesos en ejecución. *(RFC 3227 §2.1)*
- [ ] **21.** Proceder finalmente, tras los datos volátiles, a la adquisición de almacenamiento persistente (discos duros locales y externos). *(RFC 3227 §2.1)*