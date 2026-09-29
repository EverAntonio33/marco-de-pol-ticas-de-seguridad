# **Marco de Políticas de Seguridad de la Información para MiPyMEs**

## **4.1. Introducción y Alcance**

Las Micro, Pequeñas y Medianas Empresas (MiPyMEs) representan un objetivo altamente atractivo para los ciberdelincuentes debido, con frecuencia, a la falta de controles formales de seguridad. El presente **Marco de Políticas de Seguridad de la Información** establece las directrices pragmáticas, normativas y organizativas necesarias para proteger los activos de información, garantizar la continuidad del negocio y mitigar los riesgos cibernéticos sin comprometer la agilidad operativa de la empresa.

## **4.2. Estructura Jerárquica de la Documentación de Seguridad**

Para garantizar un marco normativo claro, la documentación de seguridad se organiza en cuatro niveles:

                  \+-----------------------------------+  
                  |  1\. Política General de Seguridad |  \<-- Directrices estratégicas  
                  \+-----------------------------------+  
                                    |  
                  \+-----------------------------------+  
                  |   2\. Políticas Específicas        |  \<-- Normas temáticas  
                  \+-----------------------------------+  
                                    |  
                  \+-----------------------------------+  
                  |   3\. Procedimientos y Guías       |  \<-- "Paso a paso" operativo  
                  \+-----------------------------------+  
                                    |  
                  \+-----------------------------------+  
                  |   4\. Registros y Evidencias       |  \<-- Auditoría y control  
                  \+-----------------------------------+

## **4.3. Políticas Específicas de Seguridad**

### **Política 1: Control de Acceso y Gestión de Identidades**

* **Principios Clave:**  
  * **Mínimo Privilegio:** Cada colaborador tendrá acceso únicamente a la información y sistemas estrictamente necesarios para el desempeño de sus funciones.  
  * **Autenticación Fuerte:** Es obligatorio el uso de Autenticación de Doble Factor (MFA / 2FA) en todas las cuentas corporativas (correo electrónico, almacenamiento en la nube, acceso a servidores).  
  * **Gestión de Contraseñas:**  
    * Longitud mínima de 12 a 16 caracteres.  
    * Combinación de mayúsculas, minúsculas, números y símbolos.  
    * Prohibición del uso de contraseñas personales o reutilizadas.  
    * Uso recomendado de un gestor de contraseñas empresarial.  
  * **Baja de Usuarios (Offboarding):** Desactivación inmediata de cuentas e accesos el mismo día en que finalice la relación laboral de un empleado o contratista.

### **Política 2: Seguridad en Puestos de Trabajo y Dispositivos Móviles**

* **Uso de Equipos Corporativos:**  
  * Bloqueo de pantalla automático tras 3 a 5 minutos de inactividad.  
  * Prohibición de instalación de software no autorizado (principio de lista blanca o restricción de permisos de administrador local).  
  * Antivirus/EDR actualizado obligatoriamente en todos los endpoints.  
* **Política de "Escritorio Limpio" (Clean Desk):** No dejar documentos impresos confidenciales ni credenciales escritas en papel sobre los escritorios.  
* **Política BYOD (Bring Your Own Device):**  
  * Si los empleados usan dispositivos personales para consultar correo o datos de la empresa, el dispositivo debe contar con PIN/patrón de bloqueo y cifrado de disco activado.

### **Política 3: Gestión de Respaldo y Copias de Seguridad (Backup)**

* **Regla 3-2-1:**  
  * **3** copias de los datos críticos.  
  * **2** medios de almacenamiento distintos (ej. servidor local y almacenamiento cloud).  
  * **1** copia fuera de la red principal o inmutable (offline / air-gapped) para prevenir el cifrado por Ransomware.  
* **Frecuencia:** Respaldos automáticos diarios para bases de datos transaccionales y semanales/mensuales para archivos generales.  
* **Pruebas de Restauración:** Realizar simulacros de restauración de datos como mínimo cada trimestre para validar la integridad de las copias.

### **Política 4: Uso Aceptable de Redes y Comunicaciones**

* **Uso del Correo Electrónico:** Prohibido el uso del correo institucional para registros personales o sitios no laborales.  
* **Redes Wi-Fi Corporativas:**  
  * Separación estricta de la red Wi-Fi de empleados y la red Wi-Fi de Invitados (*Guest*).  
  * Cifrado WPA3 o WPA2-Enterprise para la red interna.  
* **Uso de Redes Públicas / Teletrabajo:** Obligatoriedad de utilizar una red privada virtual (VPN) corporativa cifrada para acceder a recursos internos cuando se trabaje de forma remota.

### **Política 5: Gestión de Vulnerabilidades y Actualizaciones**

* **Parches de Seguridad:** Aplicación automática o programada de parches del sistema operativo (Windows, Linux, macOS) y aplicaciones críticas (navegadores, suites ofimáticas) dentro de los primeros 14 días tras su liberación.  
* **Cierre de Puertos Innecesarios:** Bloqueo de puertos no utilizados en routers/firewalls (ej. RDP 3389 público, FTP 21\) para reducir la superficie de ataque.

### **Política 6: Respuesta a Incidentes y Concienciación**

* **Reporte de Incidentes:** Todo colaborador que detecte un correo sospechoso (Phishing), pérdida de un dispositivo o comportamiento anómalo debe notificarlo de inmediato al área de TI o al responsable de seguridad.  
* **Plan de Concienciación Continuo:**  
  * Capacitaciones cortas trimestrales sobre ingeniería social y Phishing.  
  * Simulaciones periódicas de prueba de Phishing.

## **4.4. Matriz de Roles y Responsabilidades (RACI)**

| Rol / Función | Dirección / Gerencia | Responsable de TI / Seguridad | Empleados / Usuarios | Proveedores Externos |
| :---- | :---- | :---- | :---- | :---- |
| **Aprobación de Políticas** | **A / R** | C | I | I |
| **Implementación Técnica** | I | **R** | C | C |
| **Cumplimiento Diario** | I | A | **R** | **R** |
| **Reporte de Incidentes** | I | **A** | **R** | **R** |

**Leyenda RACI:**

* **R (Responsible):** Quien ejecuta la tarea.  
* **A (Accountable):** Quien rinde cuentas y aprueba el resultado final.  
* **C (Consulted):** Quien aporta información relevante.  
* **I (Informed):** Quien es notificado del avance/resultado.

## **4.5. Hoja de Ruta para la Implementación en la MiPyME**

1. **Fase 1 (Mes 1):** Diagnóstico inicial, aprobación de la Política General y habilitación de MFA en correo corporativo.  
2. **Fase 2 (Mes 2):** Configuración de política de copias de seguridad 3-2-1 y despliegue de Antivirus/EDR centralizado.  
3. **Fase 3 (Mes 3):** Sensibilización al personal en Phishing e ingeniería social.  
4. **Fase 4 (Continuo):** Auditorías periódicas, revisión de logs y pruebas de restauración de respaldos.