# Redes

## Qué son las redes

De una manera más coloquial podemos decir que las redes es el medio que se crea cuando un servidor trabaja con un cliente, lo que en un término más técnico es cuando el *hardware* comparte recursos y utiliza servicios como lo es el *software*

## Modelo *OSI*

El modelo *OSI (Open Systems Interconnection)* proporciona un modelo estándar para que los sistemas informáticos se puedan comunicar entre sí.

### Capas del modelo *OSI*
1. Capa Física
    - *Hubs* y cables de red.
1. Capa de Enlace de datos.
    - Define el formato de los datos en la red
        - *MAC*:La dirección *MAC* se asigna al conectarse a la red es utilizada para identificar y enviar los datos.
        - *LLC*: Aquí tenemos el control del flujo de los datos en la red.
1. Capa de Red.
    - Controla el envío entre el origen y el destino del paquete
        - Dirección *IP*: Es la identificación de la máquina en la red.
1. Capa de Transporte.
    - cOntrola la recepción de los paquetes o datos enviados en la capa anterior.
1. Capa de Sesión.
    - Es la responsable de crear la conexión entre *hosts*.
1. Capa de Presentación.
    - Es la que traduce de códigos a caracteres que se mandarán hacía la siguiente capa.
1. Capa de Aplicación.
    - Es la capa con la que el usuario interáctua de manera directa, algo que conocemos como el *frontend*.

[Para conocer más sobre las capas del Sistema *OSI* da *clic* en este *link*](https://www.youtube.com/watch?v=E7H5xcIudhA)

## Tipos de Redes

### Por Topología


 - Bus        
 - Anillo    
 - Estrella   
 - Malla    

 ![Topologías](https://www.mindomo.com/preview.htm?m=8acfa98a155b4f95be1d36d341bede50) 

### Área de alcance

| Nombre del tipo de Red | Descripción  | 
| --------- | --------- |
| LAN (*local Area Network*)           |     Una red pequeña que funciona para conectar ordenadores dentro de una casa o empresa                     |   
| WLAN (*Wireless Local Area Network*)     |  Es, al igual que el anterior una red pequeña, pero en lugar de conectarse a la red por medio de cable se conecta por *wi-fi*.                        |    
| MAN (*Metropolitan Area Network*)   | Es la que se establece cuando una compañía de red ofrece un servicio y comienza a conectar y proporcionar conexión a la red en una colonia                          |    
| WAN (*Wide Area Network*)      | Es la que despliegan las empresas para proporcionar red a una zona más amplia, como un país                         |    
| SAN (*Storage Area Network*)      | Es una red donde un usuario se conecta a un servidor el cual almacena y guarda datos                         |    