# Capa de Acceso a la Red (Ethernet)

En este módulo he profundizado en cómo funciona Ethernet, el estándar más utilizado en las redes LAN. Como analista de seguridad, entender esta capa es crítico para detectar ataques de red local.

## Conceptos Clave Aprendidos

1. La Subcapa MAC y LLC
Ethernet divide la Capa 2 en dos:
LLC (Logical Link Control): Se comunica con las capas superiores (Capa 3).
MAC (Media Access Control): Se encarga del hardware y de colocar los datos en el cable.

2. El Switch: El cerebro de la LAN
Aprendí cómo un Switch construye su Tabla de Direcciones MAC:
- Cuando llega una trama, el switch anota la MAC de origen y el puerto por donde entró.
- Si no conoce la MAC de destino, hace un Flood (envía la trama por todos los puertos excepto por donde vino).

3. Métodos de Conmutación
Store-and-Forward: El switch recibe toda la trama y verifica que no tenga errores antes de enviarla (Más seguro).
Cut-Through: Envía la trama en cuanto lee la dirección de destino (Más rápido, pero puede enviar errores).
