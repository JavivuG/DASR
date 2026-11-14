# DASR — Diseño, Administración y Seguridad de Redes

Diseño y simulación en Cisco Packet Tracer de la red empresarial de una compañía ficticia con cuatro sedes, junto con las prácticas en las que se trabajó cada tecnología que usa.

> Asignatura **Diseño, Administración y Seguridad de Redes** · 3.º curso, 1.er cuatrimestre · Curso 2023-2024 · Grado en Ingeniería Informática, Universidad de Valladolid.

## Qué hace

**Proyecto final (Grupo 04).** Red para la empresa que da soporte al agente conversacional ficticio *ChatCyL*:

- Oficinas en **Valladolid, Salamanca, León y Burgos**, unidas por enlaces punto a punto, y una conexión dedicada con **SCAYLE** para almacenamiento y cómputo.
- **Segmentación por VLAN** según el departamento (investigación, comercial, gestión, TI, etc.), para que cada grupo de usuarios acceda solo a su subred.
- Red cableada y **WiFi** para empleados y visitas en todas las oficinas, con autenticación de usuarios en la red.
- Portal del empleado y portal web con una demo de ChatCyL en una **DMZ**, separados de la red interna.
- Documentación en tres entregas: memoria del Hito 1, memoria del Hito 2 e informe técnico final.

**Prácticas de la asignatura:**

| Carpeta | Contenido |
|---------|-----------|
| [Practica_0](Practica_0/) | Guion y escenario inicial (`p0.pkt`) |
| [Practica_1](Practica_1/) | VTP y PVST: escenarios con STP activado, desactivado y en modo *rapid* |
| [Practica_2](Practica_2/) | Redundancia de puerta de enlace con HSRP, con capturas de las pruebas de ping normales y con fallos |
| [Practica_guiada_1](Practica_guiada_1/) | Listas de control de acceso (ACL) |
| [Practica_guiada_2](Practica_guiada_2/) | DNS y NAT |
| [Practica_guiada_3](Practica_guiada_3/) | Conmutación multicapa (MLS) |
| [Practica_guiada_4](Practica_guiada_4/) | Port Security y 802.1X |
| [Practica_guiada_5](Practica_guiada_5/) y [6](Practica_guiada_6/) | Enrutamiento |
| [Practica_guiada_7](Practica_guiada_7/) | Gestión de red |
| [Practica_guiada_8](Practica_guiada_8/) | Redes inalámbricas (WiFi) |

Cada práctica guiada contiene la actividad de Packet Tracer (`.pka`) y el PDF de capturas entregado.

## Tecnologías

- **Dispositivos**: routers y switches Cisco, servidores de red, controlador inalámbrico (WLC) y puntos de acceso ligeros (LAP)
- **Enrutamiento**: EIGRP con rutas sumarizadas en las capas de distribución y núcleo; enrutamiento estático para la salida a Internet y hacia SCAYLE
- **Direccionamiento**: DHCP para la asignación automática de direcciones y NAT para el acceso a Internet desde la red interna
- **Servicios**: DNS; HTTP/HTTPS para el portal del empleado y la demo de ChatCyL
- **Seguridad**: VLAN, ACL, Port Security, autenticación 802.1X con RADIUS y SNMPv3 (gestión con cifrado)
- **Herramienta**: Cisco Packet Tracer

## Aspectos técnicos destacados

- **Diseño jerárquico** con capas de núcleo y distribución, en las que se sumarizan las rutas EIGRP para reducir el tamaño de las tablas de enrutamiento.
- **Seguridad por capas**: VLAN por departamento, ACL entre subredes, autenticación con RADIUS en los switches y en la WLAN, y servicios públicos aislados en una DMZ.
- **Salida controlada**: NAT y rutas estáticas para la salida a Internet y hacia SCAYLE, que mejoran la seguridad del perímetro.
- **Diseño a partir de requisitos**: el informe parte de requisitos de negocio y técnicos (los críticos, marcados) y de ellos deduce el diseño de la red.

## Estructura del repositorio

```text
DASR/
├── Practica_0/ … Practica_2/          # Prácticas evaluables (.pkt + guion/entrega en PDF)
├── Practica_guiada_1/ … _8/           # Prácticas guiadas (.pka + capturas en PDF)
└── Proyecto/
    ├── Hito_1/memoria_Grupo4.pdf
    ├── Hito_2/memoria_grupo4.pdf
    └── Entrega_final/
        ├── informe_Grupo4.pdf         # Informe técnico final
        └── red_Grupo4.pkt             # Red completa en Packet Tracer
```

## Requisitos

- [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) (los ficheros `.pkt` y `.pka` solo se abren con esta herramienta)
- [Git](https://git-scm.com/) para clonar el repositorio

## Cómo abrir los proyectos

```bash
git clone https://github.com/JavivuG/DASR.git
cd DASR
```

Abre [`Proyecto/Entrega_final/red_Grupo4.pkt`](Proyecto/Entrega_final/red_Grupo4.pkt) en Packet Tracer para ver la red completa, y consulta el [informe final](Proyecto/Entrega_final/informe_Grupo4.pdf) para el diseño y las pruebas. Las prácticas se abren del mismo modo desde su carpeta. No se ha comprobado la compatibilidad con versiones concretas de Packet Tracer.

## Autoría

El proyecto final se hizo en grupo (Grupo 04). Los integrantes figuran en el [informe final](Proyecto/Entrega_final/informe_Grupo4.pdf). Las prácticas son de Javier García González.

---

Forma parte de [UVa-Projects](https://github.com/JavivuG/UVa-Projects).
