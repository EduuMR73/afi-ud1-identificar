# Lista de Comprobación Forense

Herramienta de trabajo para una escena real de identificación y preservación. Fuentes: RFC 3227, NIST SP 800-86 y manual de buenas prácticas ENFSI para el examen forense de tecnología digital.

## 1. Al llegar
- [ ] **1.** Confirmar la autorización escrita: qué equipos, cuentas y personas cubre. No tocar dispositivos personales ni de terceros sin su consentimiento o un mandato. *(RFC 3227 §2.3; NIST SP 800-86 §3.1.1)*
- [ ] **2.** Preparar antes de intervenir herramientas validadas, cámara, bolsas y etiquetas de embalaje y formularios de custodia. *(ENFSI §9.1; NIST SP 800-86 §3.1.2)*
- [ ] **3.** Asegurar el perímetro físico, limitar el acceso a la zona y anotar quién tiene acceso a cada equipo. *(ENFSI §8.2; NIST SP 800-86 §3.1.3)*
- [ ] **4.** Fotografiar y documentar la escena completa antes de mover nada: pantallas, cables, periféricos y sesiones abiertas. *(NIST SP 800-86 §3.1.2; ENFSI §8.2)*
- [ ] **5.** Observar el estado de cada equipo (encendido, apagado, bloqueado, salvapantallas) sin interactuar con él. *(NIST SP 800-86 §3.1.2; ENFSI §9.2)*
- [ ] **6.** Localizar dispositivos y soportes a la vista (móviles, discos externos, USB, impresoras) y evidencias físicas asociadas (notas con contraseñas, agendas, manuales). *(NIST SP 800-86 §3.1.1; ENFSI §9.2)*
- [ ] **7.** Aislar de la red los móviles de la empresa (bolsa Faraday o modo avión) para evitar borrados remotos, y mantenerlos cargados. Los personales, solo con consentimiento (punto 1). *(ENFSI §8.2; NIST SP 800-86 §2.1 y §3.1.3)*
- [ ] **8.** Anotar quién está presente, qué hace y qué observa, e impedir que la persona investigada use los equipos. *(RFC 3227 §3.2; NIST SP 800-86 §3.1.3)*

## 2. Antes de tocar nada
- [ ] **9.** Trazar la topología de red física (routers, puntos de acceso, switches, cableado) y los equipos conectados. *(NIST SP 800-86 §3.1.1; RFC 3227 §2.1)*
- [ ] **10.** Identificar la infraestructura local no visible: servidores de ficheros, NAS y otros almacenamientos en red. *(NIST SP 800-86 §3.1.1)*
- [ ] **11.** Preguntar a TI y a la gerencia por las fuentes fuera de la oficina (nube, VPN, correo, administración del edificio) y por quién es el propietario de cada una. *(NIST SP 800-86 §3.1.1)*
- [ ] **12.** Preguntar por las copias de seguridad: qué se copia, con qué frecuencia y cuánto tiempo se conservan. *(NIST SP 800-86 §3.1.1 y §2.4.3)*
- [ ] **13.** Preguntar qué sistemas generan registros (cortafuegos, VPN, impresoras, cámaras, auditoría de correo y nube) y cuánto tiempo los conservan antes de sobrescribirlos. *(NIST SP 800-86 §3.1.2, §6.2.1 y §6.2.4)*
- [ ] **14.** Comprobar si los equipos usan cifrado (BitLocker, FileVault) y dónde están las claves de recuperación antes de decidir apagar o desmontar nada. *(RFC 3227 §2.2; NIST SP 800-86 §3.2)*

## 3. Al decidir qué se adquiere y en qué orden
- [ ] **15.** Decidir, con la gerencia, si la evidencia debe poder usarse en un proceso legal o disciplinario. Ante la duda, preservar. *(NIST SP 800-86 §3.1.2; RFC 3227 §3.2)*
- [ ] **16.** Valorar cada fuente por su valor probable, su volatilidad y el esfuerzo necesario para adquirirla, y dejar por escrito el orden resultante. Repartir el trabajo en paralelo entre sistemas distintos, pero paso a paso dentro de cada uno. *(NIST SP 800-86 §3.1.2; RFC 3227 §2)*
- [ ] **17.** Dar prioridad a lo que se pierde con el paso del tiempo aunque no sea memoria: registros que se sobrescriben, copias que rotan, grabaciones que caducan. *(NIST SP 800-86 §3.1.2)*
- [ ] **18.** No apagar ni reiniciar ningún equipo encendido hasta terminar la recogida de datos volátiles. *(RFC 3227 §2.2)*
- [ ] **19.** En cada equipo encendido, capturar primero el estado de red: conexiones activas, caché ARP y tabla de rutas. *(RFC 3227 §2.1; NIST SP 800-86 §5.2.1)*
- [ ] **20.** Tras capturar el estado de red, retirar las vías externas de alteración del equipo (cable de red, Wi-Fi), teniendo presente que desconectar puede activar mecanismos de borrado y valorando el impacto en el resto de la oficina. *(RFC 3227 §2.2 y §3.2; NIST SP 800-86 §3.1.3)*
- [ ] **21.** Capturar a continuación la memoria (RAM) y los procesos con herramientas desde un soporte protegido, sin instalar nada en el equipo. *(RFC 3227 §2.1, §2.2 y §5; NIST SP 800-86 §5.2.1)*
- [ ] **22.** Dejar para el final los discos y soportes persistentes, adquiridos mediante copia bit a bit y trabajando solo sobre la copia. *(RFC 3227 §2.1; NIST SP 800-86 §4.2.1)*
- [ ] **23.** Llevar un registro detallado, con fecha y hora, de cada comando y cada decisión, indicando la diferencia entre el reloj del sistema y UTC. *(RFC 3227 §2 y §3.2; NIST SP 800-86 §3.1.2)*
- [ ] **24.** Calcular el hash de cada adquisición, etiquetar cada elemento y documentar la cadena de custodia: quién, cuándo, dónde y cómo se guarda. *(NIST SP 800-86 §3.1.2; RFC 3227 §3.2 y §4.1)*