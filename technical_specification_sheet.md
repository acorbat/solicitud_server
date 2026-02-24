# **Especificaciones Técnicas: Servidor de Procesamiento de Bioimágenes**

**Destino:** Universidad de Buenos Aires (UBA)

**Proyecto:** Omero \+ Análisis de Imágenes

**Fecha:** 24 de febrero de 2026

## **1. Resumen Ejecutivo**

Se solicita la adquisición de un servidor de cómputo de alto rendimiento (HPC) diseñado para el procesamiento y análisis de grandes volúmenes de datos provenientes de bioimágenes (confocal, light-sheet, etc.). El equipo debe ser "GPU-Ready" para permitir la expansión futura con placas de aceleración gráfica para Deep Learning.

## **2. Especificaciones Técnicas Requeridas**

### **2.1. Desglose de Costos Estimados (USD)**

| Component | Estimated Cost (New) | Notes |
| :---- | :---- | :---- |
| **Chassis & Motherboard** | $2,500 – $4,000 | Includes redundant power supplies (750W–1100W). |
| **CPU (32 Cores Total)** | $3,500 – $6,000 | Can be a single AMD EPYC (e.g., 9354\) or dual Intel Xeon Golds. |
| **RAM (128 GB DDR5)** | $1,200 – $2,000 | Usually 4x32GB or 8x16GB RDIMMs for performance. |
| **Storage (Base)** | $800 – $1,500 | 2x 480GB NVMe/SAS SSDs (RAID 1 for OS). |
| **Support (3-Year Next-Business-Day)** | $1,000 – $2,500 | Essential for university uptime requirements. |
| **Total Estimate** | **$9,000 – $16,000** | **Before university discounts.** |

---

### **2.2. Detalle de Partes Necesarias (Bill of Materials)**

Para que el servidor sea funcional y apto para bioimágenes en la UBA, el pliego debe incluir estas partes específicas:

#### **A. Núcleo de Cómputo y Memoria**

* **Procesador:** 1x AMD EPYC 9354 (32 núcleos, 3.25GHz) o equivalente Intel Xeon Gold. Debe soportar PCIe Gen5 para futuras GPUs.  
* **Memoria:** 128 GB (Mínimo 8 x 16GB RDIMM, 4800MT/s o superior) para ocupar todos los canales de memoria del CPU.

#### **B. Chasis y Expansión (Crucial para GPU)**

* **Chasis:** Formato 2U con bahías de 2.5" (SFF).  
* **GPU Enablement Kit:** Debe especificar "GPU Ready". Esto incluye:  
  * **Risers PCIe:** Soportes físicos para conectar placas de video de doble ancho.  
  * **Power Cables:** Cables de alimentación internos (8-pin/12-pin) específicos para el servidor.  
  * **Ventiladores de Alto Rendimiento:** Necesarios para disipar el calor extra de una futura GPU.  
* **Fuentes de Poder:** 2x 1100W o 1400W (Redundantes, Hot-plug). Las fuentes estándar de 750W no soportan GPUs de alta gama.

#### **C. Almacenamiento de Bioimágenes**

* **Drive 1 & 2 (OS):** 2x 480GB SSD SATA/NVMe en RAID 1 (Espejo para el sistema operativo).  
* **Drive 3 & 4 (Datos):** 2x 2TB NVMe PCIe Gen4/5 Enterprise SSD. Configurados en RAID 0 para máxima velocidad de lectura/escritura en procesamiento de imágenes.  
* **Controladora RAID:** Hardware RAID con cache y batería (ej. PERC H755 o HPE Smart Array) si se opta por discos SAS/SATA. Para NVMe puro, se usa VROC o passthrough directo.

#### **D. Accesorios de Instalación**

* **Rieles de Rack:** Sliding Rails with Cable Management Arm (para facilitar el mantenimiento en el data center).  
* **Bisel de Seguridad:** Front Bezel con cerradura.  
* **Tarjeta de Red:** Dual Port 10GbE SFP+ (las bioimágenes son muy pesadas para redes de 1GbE).

---

### **2.3. Sugerencia de Proveedores para UBA**

En Argentina, las licitaciones de UBA suelen ser ganadas por integradores locales que manejan el beneficio de ROECyT. Algunos de los más comunes para Dell, HPE o Lenovo son:

* **Microglobal**  
* **Air Computers**  
* **TelexTorage**  
* **DataStar**

## **4. Justificación Técnica de los Componentes Seleccionados**

La configuración de hardware propuesta responde a las exigencias computacionales específicas del procesamiento de imágenes biológicas de alta resolución (Confocal, Light-sheet, STED, etc.) y garantiza la viabilidad del proyecto a largo plazo.

### **4.1. Procesador de 32 Núcleos (CPU)**

El procesamiento de bioimágenes moderno utiliza algoritmos de deconvolución y reconstrucción 3D que son altamente paralelizables. Un mínimo de 32 núcleos permite:

* Reducir los tiempos de procesamiento de horas a minutos en tareas de renderizado volumétrico.  
* Ejecutar múltiples procesos de análisis en paralelo sin saturar el sistema operativo.  
* Soporte para software de código abierto (ej. ImageJ/Fiji, Ilastik) que aprovecha el multithreading.

### **4.2. Memoria RAM de 128 GB DDR5**

Las bioimágenes suelen generar archivos "stacks" de varios gigabytes.

* Carga en memoria: Para evitar cuellos de botella, el dataset completo debe cargarse en la RAM. 128 GB permiten trabajar con volúmenes de datos complejos sin recurrir al intercambio en disco (swapping), lo cual degradaría el rendimiento.  
* Arquitectura de Canales: La configuración de 8 módulos optimiza el ancho de banda entre el CPU y la memoria, esencial para el flujo de datos masivo de las cámaras científicas.

### **4.3. Almacenamiento NVMe de Alta Velocidad (4 TB)**

El almacenamiento basado en discos mecánicos o SSDs SATA tradicionales es insuficiente para la bioinformática actual.

* Velocidad de Escritura: Las imágenes se generan a tasas muy altas; los discos NVMe aseguran que no se pierdan datos durante la adquisición.  
* Velocidad de Lectura: Agiliza el acceso aleatorio a los píxeles durante el entrenamiento de modelos de IA o el filtrado de imágenes de gran tamaño.

### **4.4. Chasis 2U y Kit "GPU-Ready" (Escalabilidad)**

La investigación biomédica actual depende cada vez más del Deep Learning para la segmentación y clasificación automática (ej. Cellpose, StarDist).

* Futuro Cómputo: Aunque inicialmente no se adquiera la GPU, el chasis de 2U y las fuentes de 1100W+ son obligatorios para albergar placas de video de grado científico (como la serie NVIDIA RTX A o L) que requieren gran espacio físico y refrigeración dedicada.  
* Ahorro de Costos: Adquirir el kit de habilitación (risers y cables) de fábrica evita que el servidor quede obsoleto en menos de un año o que su actualización futura sea técnicamente inviable por falta de partes específicas del fabricante.

### **4.5. Conectividad 10GbE**

Dado el tamaño de los archivos de bioimágenes, una red estándar de 1GbE es un cuello de botella crítico. La placa de 10GbE es indispensable para transferir los datos generados desde el microscopio hacia el servidor y para el respaldo de datos en los servidores centrales de la UBA de manera eficiente.

### **4.6. Garantía On-Site (Siguiente Día Hábil)**

Dada la naturaleza crítica de la investigación científica, la disponibilidad del equipo es prioritaria. Una falla en un componente no debe detener la actividad del servicio por semanas; por ello se justifica la garantía del fabricante con reemplazo de partes en el lugar de instalación.

## **5. Requisitos de Garantía y Soporte**

* **Garantía:** Mínimo 3 años de soporte técnico del fabricante en sitio (On-site).  
* **Certificaciones:** El equipo debe ser compatible con entornos Linux (Ubuntu/CentOS) y Windows Server.

## **6. Notas para Adquisición (Ley ROECyT)**

Considerando que el destino es la Universidad de Buenos Aires, el oferente deberá facilitar la documentación necesaria para tramitar la exención de derechos de importación e IVA bajo el régimen de la **Ley 25.613 (Certificado ROECyT)**, en caso de que el equipo sea importado específicamente para este fin científico.