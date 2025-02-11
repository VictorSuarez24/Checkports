# 🛡️ CheckPorts - Análisis de Seguridad de Puertos

**CheckPorts** es una herramienta diseñada para realizar análisis de seguridad en redes, enfocado en escanear puertos abiertos, realizar escaneos en modo sigiloso para evadir detección y detectar IPs maliciosas que intentan acceder a un sistema. Está pensado para ser utilizado por administradores de sistemas y profesionales de ciberseguridad.

## 🚀 Funcionalidades

- **Escaneo de puertos abiertos:** Detecta puertos abiertos en el sistema y muestra los servicios asociados a cada puerto.
- **Escaneo sigiloso (stealth mode):** Utiliza herramientas como `nmap` para escanear puertos sin ser detectado, ideal para análisis de penetración.
- **Detección y bloqueo de IPs maliciosas:** Detecta intentos de acceso fallidos (por ejemplo, en SSH) y bloquea las IPs que han superado un número determinado de intentos fallidos.

## 📋 Requisitos

- Linux (Distribuciones basadas en Debian preferentemente)
- `nmap`
- `ss`
- `getent`
- `iptables` (para bloquear IPs)
- Acceso a logs del sistema (por ejemplo, `/var/log/auth.log`)

## 🔧 Instalación

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/VictorSuarez24/checkports.git
   cd checkports
