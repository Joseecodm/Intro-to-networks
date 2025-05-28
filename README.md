# JLaboratories — Configuración de Red

Este repositorio contiene la configuración de red necesaria para desplegar la aplicación **JLaboratories** en un entorno cliente-servidor sobre LAN.

---

## 1. Descripción de la Subred

- **Rango IPv4**: `172.16.0.64/27`  
- **Máscara**: `255.255.255.224`  
- **Puerta de enlace**: `172.16.0.126`  

---

## 2. Direcciones IP de los Dispositivos

| Dispositivo         | IPv4          | Máscara           | Gateway        | IPv6                   |
|---------------------|---------------|-------------------|----------------|------------------------|
| **PC1 (Servidor)**  | 172.16.0.97   | 255.255.255.224   | 172.16.0.126   | 2001:db8:1:d::97/64    |
| **PC2 (Cliente)**   | 172.16.0.98   | 255.255.255.224   | 172.16.0.126   | 2001:db8:1:d::98/64    |
| **Switch (SW1)**    | N/A (gestión) | 255.255.255.224   | N/A            | 2001:db8:1:d::2/64     |
| **Router (R1)**     | 172.16.0.126  | 255.255.255.224   | N/A            | 2001:db8:1:d::1/64     |

---

![Topología de red de JLaboratories](Pictures/Topology.png)
