
LabSec Lab Environment

Laboratorio de infraestructura y ciberseguridad diseñado como una red y sandbox general para desarrollar múltiples laboratorios y escenarios de prueba.

El entorno busca simular una pequeña infraestructura empresarial sobre la cual experimentar con administración de sistemas, redes, seguridad, monitoreo, detección y respuesta ante incidentes.

La infraestructura combina máquinas virtuales con dispositivos de red virtualizados mediante GNS3, proporcionando una base reutilizable para diferentes proyectos y experimentos.


Objetivos.

Crear una infraestructura de red reutilizable para múltiples laboratorios.
Practicar administración de sistemas y servicios empresariales.
Experimentar con networking, segmentación y seguridad.
Construir escenarios controlados para pruebas de ciberseguridad.
Integrar herramientas de monitoreo y detección.
Simular incidentes y practicar su investigación.
Mantener un entorno aislado para probar nuevas tecnologías y herramientas.


Componentes actuales.

-Infraestructura de red.
GNS3.
Firewall/router virtualizado.
Switching y routing.
Segmentación de red mediante VLANs.
NAT y acceso a Internet.
Redes independientes para Management, Servers, Users y Security.

-Infraestructura Windows.
Windows Server.
Active Directory Domain Services.
DNS.
DHCP.
Group Policy.
Windows workstation.
File Server.

-Seguridad y monitoreo.
Wazuh SIEM.
Recolección de eventos de Windows.
Monitoreo de endpoints.
Análisis de eventos de seguridad.


Filosofía del laboratorio.

El objetivo no es simplemente mantener una infraestructura permanente, sino utilizarla como una plataforma experimental reutilizable.
Los componentes pueden activarse, modificarse o reemplazarse dependiendo del laboratorio que se quiera realizar, permitiendo construir diferentes escenarios sobre una misma infraestructura base.
El laboratorio evolucionará progresivamente a medida que se incorporen nuevas tecnologías, herramientas y escenarios de infraestructura y ciberseguridad.