# tp2_redes
DHCP configuracion
---
## Integrantes
- Isabella Murioni
- Lucia Saint Martin
---
## Implementación:

1. Primero instalamos packet tracer en nuestro pendrive booteable con Linux y una vez instalado, armamos la red: con 1 router, 1 switch y 2 PCs.

2. Luego, conectamos los dispositivos. Para realizar las conexiones de la red, utilizamos cables de cobre, que son los más comunes en este tipo de configuraciones (representados por líneas negras continuas). El router se conectó al switch mediante el puerto FastEthernet0/0 del router hacia el puerto FastEthernet0/3 del switch. Luego, conectamos las PCs al switch utilizando los puertos FastEthernet0/1 y FastEthernet0/2 del switch, que van respectivamente a los puertos FastEthernet0 de cada computadora.

3. Una vez conectados, configuramos el router entrando a la interfaz CLI (IOS command line interface). Con este código se configura un router Cisco para que funcione como servidor DHCP en una red local. Primero se le asigna una dirección IP a la interfaz del router y se la habilita para que pueda comunicarse con otros dispositivos. Luego se establece un rango de direcciones IP que serán asignadas automáticamente a las PCs mediante el protocolo DHCP. También se configura la puerta de enlace predeterminada y un servidor DNS. Finalmente, en cada PC se selecciona la opción de obtener IP por DHCP para que reciban la configuración de red automáticamente y puedan conectarse al router y entre ellas.

4. Finalmente en cada PC, ingresas a la pestaña Desktop, luego a IP Configuration, y ahí seleccionas la opción DHCP. Al hacer esto, la PC le solicita automáticamente al router una dirección IP y otros datos de red (como la máscara de subred, la puerta de enlace y el DNS). Si el router está correctamente configurado como servidor DHCP, la PC recibirá toda esta información sin necesidad de ingresarla manualmente, quedando conectada a la red automáticamente.
