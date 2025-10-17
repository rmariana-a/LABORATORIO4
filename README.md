# LABORATORIO4
# Redes y Máquinas Virtuales  

## Elaborado por:
**Rodian Garay**  
**Mariana Lombana**

---

### 1. Comunicación por consola  
Para iniciar el laboratorio, se estableció la conexión entre el computador y el **switch Cisco 2960** utilizando un **cable de consola**.  
Desde **Ubuntu**, se accedió al dispositivo empleando el siguiente comando:  

```bash
screen /dev/ttyUSB0 9600

---
### 2. Configuración inicial del switch  
Dentro del modo de configuración, se realizó lo siguiente:  

- Asignación del **nombre de host**.  
- Establecimiento de **contraseñas de acceso**.  
- Activación de la interfaz principal.  
- Creación de la **VLAN 10** y asignación de su configuración correspondiente.  

Esto garantizó la segmentación y correcta comunicación entre los dispositivos conectados al switch.
---  

####3. Configuración de la Raspberry Pi  

Se configuró la interfaz de red de la **Raspberry Pi** con una **dirección IP estática** dentro del rango asignado a la **VLAN 10**, garantizando su correcta comunicación con los demás equipos del laboratorio.  

**Configuración en consola:**  
```bash
sudo nano /etc/dhcpcd.conf


