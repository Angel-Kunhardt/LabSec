
DC01 y DC02 (Windows Server 2025)
- OU creadas.
- Usuarios creados.
- GPO basicas creadas (polica de contraseña, wallpaper, file server share, WSUS).
- DHCP creado para la red de usuario.

SRV01 (Windows Server 2025)
- File Server configurado para cada departamento con su respectiva file screening y cuota.
- Windows Server Update Service configurado y sincronizado.

SEC01 (Linux Ubuntu Server 26.04)
- Wazuh manager, Wazuh indexer, Wazuh dashboard, instalado.
- Agentes instalados en todos los servidores.
- Logs de Pfsense estan siendo recibidos mediante syslog.

Pfsense firewall.
- interfaces configuradas.
- Syslog configurado para enviar logs a Wazuh.
- reglas basicas de conectividad en el firewall.

