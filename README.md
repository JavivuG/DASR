# Proyecto DASR - Diseño, Administración y Seguridad de Redes (Curso 2023-2024)

Este repositorio contiene el código y la documentación del proyecto final de la asignatura **Diseño, Administración y Seguridad de Redes** (DASR) correspondiente al curso 2023-2024.

## Tabla de Contenidos
- [Descripción](#descripción)
- [Objetivos](#objetivos)
- [Tecnologías](#tecnologías)
- [Instalación](#instalación)

## Descripción

En este repositorio están las prácticas guiadas y las prácticas normales que constan de ejercicios de aprendizaje de las distintas tecnologias y protocolos de red que se usan en el proyecto final de la asignatura. Este proyecto final es bastante elaborado y, como he mencionado, consta de la gran mayoría de las tecnologías aprendidas.

## Objetivos

- Diseñar una red escalable y eficiente que cumpla con los requerimientos de una empresa ficticia.
- Implementar la configuración de dispositivos de red (routers, switches, firewalls).
- Aplicar políticas de seguridad para proteger la red contra amenazas internas y externas.
- Monitorizar el rendimiento de la red y realizar ajustes para optimizar su funcionamiento.
- Documentar las configuraciones, pruebas de seguridad y rendimiento.

## Tecnologías

Durante el curso se ha aprendido diferentes protocolos de red y tecnologías a continuación, enumero algunos de los usados en el proyecto final:
- Dispositivos de Red: Routers Cisco, Switches Cisco, Servidores de Red
- Protocolos de Enrutamiento:
    - EIGRP: Protocolo de enrutamiento dinámico para el intercambio eficiente de rutas entre routers.
    - Enrutamiento estático: Utilizado para la salida a Internet, mejorando la seguridad.
- Protocolos de Asignación de Direcciones:
    - DHCP: Asignación automática de direcciones IP a los dispositivos conectados a la red.
    - NAT: Traducción de direcciones de red para permitir la conexión a Internet desde la red interna.
- Servicios de Nombres:
    - DNS: Sistema de nombres de dominio que traduce nombres de host en direcciones IP.
- Protocolos de Seguridad:
    - Port Security: Seguridad a nivel de puerto en switches para limitar dispositivos no autorizados.
    - 802.1X: Autenticación de usuarios en la red.
    - ACL (Access Control Lists): Control de acceso mediante listas de control de tráfico.
    - SNMPv3: Protocolo de gestión de red con encriptación de datos.
- Protocolos de Transferencia:
    - HTTP/HTTPS: Transferencia de datos para servicios web como el portal del empleado y la demo de ChatCyL.

## Instalación

### Requisitos previos
Para clonar y ejecutar este proyecto, necesitarás tener instaladas las siguientes herramientas:

- [Git](https://git-scm.com/)
- [Packet Tracer](https://www.netacad.com/courses/packet-tracer)

### Clonación del Repositorio

```bash
git clone https://github.com/tu-usuario/proyecto-DASR-23-24.git
cd proyecto-DASR-23-24
