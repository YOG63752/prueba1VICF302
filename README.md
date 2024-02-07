
Error: l�nea de comandos desconocida o incompleta.

USO:
   ipconfig [/allcompartments] [/? | /all | 
                                /renew [adaptador] | /release [adaptador] |
                                /renew6 [adaptador] | |
                                 /release6 [adaptador] |
                                /flushdns | /displaydns | /registerdns |
                                /showclassid adaptador |
                                /setclassid adaptador [id._clase] |
                                /showclassid6 adaptador |
                                /setclassid6 adaptador [id._clase] ]

donde
   adaptador           Nombre de conexi�n 
                      (se permiten los caracteres comod�n * y ?; consulte los
                       ejemplos)

    Opciones:
      /?               Muestra este mensaje de ayuda.
      /all             Muestra toda la informaci�n de configuraci�n.
      /release         Libera la direcci�n IPv4 para el adaptador especificado.
      /release6        Libera la direcci�n IPv6 para el adaptador especificado.
      /renew           Renueva la direcci�n IPv4 para el adaptador
                       especificado.
      /renew6          Renueva la direcci�n IPv6 para el adaptador
                       especificado.
      /flushdns        Purga la memoria cach� de resoluci�n de DNS.
      /registerdns     Actualiza todas las concesiones DHCP y vuelve a
                       registrar los nombres DNS.
      /displaydns      Muestra el contenido de la memoria cach� de resoluci�n
                       de DNS.
      /showclassid     Muestra todos los id. de clase DHCP permitidos para
                       este adaptador.
      /setclassid      Modifica el id. de clase DHCP.  
      /showclassid6    Muestra todos los id. de clase DHCP IPv6 permitidos para
                       el adaptador.
      /setclassid6     Modifica el id. de clase DHCP IPv6.


De forma predeterminada, se muestra solamente la direcci�n IP, la m�scara de
subred y la puerta de enlace predeterminada para cada adaptador enlazado con
TCP/IP.

Para Release y Renew, si no hay ning�n nombre de adaptador especificado, se
liberan o renuevan las concesiones de direcci�n IP para todos los adaptadores
enlazados con TCP/IP.

Para Setclassid y Setclassid6, si no especific� classid, se quita.

Ejemplos:
    > ipconfig                       ... Muestra informaci�n.
    > ipconfig /all                  ... Muestra informaci�n detallada.
    > ipconfig /renew                ... Renueva todos los adaptadores.
    > ipconfig /renew EL*            ... Renueva cualquier conexi�n cuyo nombre
                                         comience con EL.
    > ipconfig /release *Con*        ... Libera todas las conexiones
                                         coincidentes, por ejemplo: 
                                             "Conexi�n cableada Ethernet 1" o
                                             "Conexi�n cableada Ethernet 2".
    > ipconfig /allcompartments      ... Muestra informaci�n sobre todos 
                                         los compartimientos.
    > ipconfig /allcompartments /all ... Muestra informaci�n detallada sobre
                                         todos los compartimientos
"# prueba1VICF302" 
