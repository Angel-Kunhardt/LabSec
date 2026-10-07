
-LabSec Lab Environment

Laboratorio de ciberseguridad e infraestructura diseñado como una red y un sandbox general para desarrollar múltiples laboratorios y escenarios de prueba.

El entorno busca simular una pequeña infraestructura empresarial, proporcionando una base reutilizable sobre la cual experimentar con administración de sistemas, redes, ciberseguridad, monitoreo, detección de amenazas y respuesta a incidentes.

La infraestructura combina máquinas virtuales y dispositivos de red virtualizados mediante GNS3, con una arquitectura segmentada que permite aislar servicios y controlar el flujo de tráfico entre diferentes áreas de la red.

Objetivos

Crear una infraestructura de red reutilizable para múltiples laboratorios.
Practicar la administración de Windows Server y Active Directory.
Implementar y probar servicios de red como DNS y DHCP.
Practicar segmentación, enrutamiento, firewalls y resolución de problemas.
Crear escenarios controlados para pruebas de seguridad.
Centralizar y analizar eventos mediante herramientas como Wazuh.
Simular incidentes y practicar procesos de detección, investigación y respuesta.
Experimentar con nuevas tecnologías y herramientas sin afectar el entorno principal.


-Arquitectura

El laboratorio utiliza GNS3 como plataforma para la infraestructura de red, incluyendo firewall, switching, routing y segmentación mediante VLANs.

Las máquinas virtuales proporcionan los servicios y endpoints necesarios para construir diferentes escenarios.


-Filosofía del laboratorio

El objetivo no es únicamente desplegar servicios, sino utilizar la infraestructura como una plataforma experimental. Los componentes pueden modificarse, reemplazarse o reutilizarse dependiendo del escenario que se quiera estudiar.

Sobre esta infraestructura se pueden construir laboratorios de:

Active Directory
Windows Server
Networking
Seguridad de endpoints
SIEM y SOC
Vulnerability Management
Análisis de tráfico
Incident Response
Hardening
Malware Analysis en entornos aislados
Automatización con PowerShell y Python
Pruebas de herramientas de seguridad

El laboratorio está diseñado para evolucionar progresivamente a medida que se incorporan nuevos servicios, herramientas y escenarios.
