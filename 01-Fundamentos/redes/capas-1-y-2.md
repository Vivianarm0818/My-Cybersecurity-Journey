#  Fase 1: Capas 1 y 2 del Modelo OSI - Fundamentos de Networking

En esta primera etapa de mi formación en el curso *Networking Essentials* de Cisco, me he centrado en cómo se mueven los datos a nivel físico y de enlace. Entender esto es vital: **no puedes defender lo que no entiendes cómo se conecta.**

##  Capa 1: Capa Física (Physical Layer)
Es la base de todo. Se encarga de la transmisión de bits puros a través de un medio físico.

- **Unidad de datos (PDU):** Bits.
- **Componentes:** Cables (UTP, Fibra Óptica), conectores (RJ-45), señales eléctricas o de luz.
- **Concepto clave de seguridad:** - **Ataques de Capa 1:** El corte físico de cables, el "tapping" (intervención física del cable para copiar datos) o el uso de dispositivos como el *Rubber Ducky* que actúan a nivel de hardware.
    - **Lección:** La seguridad física es la primera línea de defensa.

##  Capa 2: Enlace de Datos (Data Link Layer)
Aquí los bits se agrupan en **Tramas (Frames)**. Es la capa que permite que los dispositivos se comuniquen en una red local (LAN).

- **Unidad de datos (PDU):** Trama (Frame).
- **Direccionamiento:** Dirección MAC (Media Access Control). Es la dirección física "quemada" en la tarjeta de red.
- **Dispositivo clave:** El **Switch**.

### 🛠️ Conceptos de Seguridad en Capa 2 (Critical para Blue Team)
1. **MAC Spoofing:** Un atacante cambia su dirección MAC para hacerse pasar por un dispositivo autorizado.
2. **ARP Poisoning:** El protocolo ARP (que traduce IPs a MACs) no tiene memoria ni autenticación. Un atacante puede engañar a mi PC diciendo que él es el router para interceptar mi tráfico (Man-in-the-Middle).
3. **Port Security:** Aprendí que en los switches Cisco se pueden bloquear puertos para que solo acepten una dirección MAC específica, evitando que extraños conecten sus laptops.

---

##  Práctica en Laboratorio
He utilizado **Cisco Packet Tracer** para:
1. Configurar un enrutador inalámbrico.
2. Configurar el direccionamiento IP y probar conectividad.
3. Conectar dispositivos a la red alámbrica e inalámbrica.
