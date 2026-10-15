
Inventario de la infraestructura del diagrama de red

1. Internet y proveedor.

- Internet: red pública/externa conectada al proveedor de servicios.

- ISP (Proveedor de Internet): equipo de borde que conecta la red interna con Internet.

- Interfaz WAN del ISP: conexión hacia Internet.

- Interfaz LAN del ISP: conexión hacia el firewall/router interno.

2. Equipos de red principales.

- Firewall/Router PfSense:

  - Función: protección perimetral y ruteo entre Internet y la LAN.

  - Conexión WAN: hacia el ISP.

  - Conexiones internas: hacia los switches de cada zona.

  - Tiene segmentación de red para las LANs internas.

3. Segmentación de red (LANs)

- LAN-Management: 10.10.10.0/24
  - Gateway: 10.10.10.1

- LAN-Servers: 10.10.20.0/24
  - Gateway: 10.10.20.1

- LAN-Users: 10.10.30.0/24
  - Gateway: 10.10.30.1

- LAN-Security: 10.10.40.0/24
  - Gateway: 10.10.40.1

4. Switches de acceso.

- ManagementSW
  - Ubicación: LAN-Management
  - Conecta: servidores de administración

- ServersSW
  - Ubicación: LAN-Servers
  - Conecta: servidores de aplicaciones y servicios

- UsersSW
  - Ubicación: LAN-Users
  - Conecta: estaciones de trabajo de usuarios

- SecuritySW
  - Ubicación: LAN-Security
  - Conecta: infraestructura de seguridad


5. Servidores y equipos finales.

- WinServer2025 (DC01)
  - Tipo: servidor Windows
  - Red: LAN-Management
  - Conectado a ManagementSW

- WinServer2025 (DC02)
  - Tipo: servidor Windows
  - Red: LAN-Management
  - Conectado a ManagementSW

- WinServer2025 (SRV01)
  - Tipo: servidor Windows
  - Red: LAN-Servers
  - Conectado a ServersSW

- Windows10 (TestADDS)
  - Tipo: estación de trabajo
  - Red: LAN-Users
  - Conectado a UsersSW

- Ubuntu Server (SEC01)
  - Tipo: servidor Linux
  - Red: LAN-Security
  - Conectado a SecuritySW

6. Resumen de la infraestructura

- 1 proveedor de internet (ISP)
- 1 firewall/router PfSense
- 4 switches de capa de acceso
- 4 redes internas/segmentadas (LAN-Management, LAN-Servers, LAN-Users, LAN-Security)
- 5 equipos finales/servidores principales
- Topología: Internet -> ISP -> Firewall/PfSense -> Switches -> Hosts

7. Observación técnica
- La infraestructura está diseñada con segmentación por funciones, lo que mejora seguridad, administración y control de tráfico.
- La separación de redes por departamentos o servicios permite aplicar políticas, accesos y monitoreo específicos por segmento.
